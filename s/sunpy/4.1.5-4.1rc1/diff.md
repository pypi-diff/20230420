# Comparing `tmp/sunpy-4.1.5.tar.gz` & `tmp/sunpy-4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-4.1.5.tar", last modified: Thu Apr 20 17:02:32 2023, max compression
+gzip compressed data, was "sunpy-4.1rc1.tar", last modified: Fri Nov  4 18:24:17 2022, max compression
```

## Comparing `sunpy-4.1.5.tar` & `sunpy-4.1rc1.tar`

### file list

```diff
@@ -1,812 +1,804 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.137222 sunpy-4.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)   235698 2023-04-20 17:01:58.000000 sunpy-4.1.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-20 17:01:58.000000 sunpy-4.1.5/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-20 17:01:58.000000 sunpy-4.1.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 17:01:58.000000 sunpy-4.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-20 17:02:32.137222 sunpy-4.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-20 17:01:58.000000 sunpy-4.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.053221 sunpy-4.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/about.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.053221 sunpy-4.1.5/docs/code_ref/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.053221 sunpy-4.1.5/docs/code_ref/coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/coordinates/carrington.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/coordinates/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/coordinates/other_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/coordinates/rotatedsunframe.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/coordinates/velocities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/coordinates/wcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/io.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/map.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/net.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/physics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/stability.rst
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/sun.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/sunpy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/sunpy_stability.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/timeseries.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/code_ref/visualization.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.053221 sunpy-4.1.5/docs/dev_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.057222 sunpy-4.1.5/docs/dev_guide/contents/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/backports.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/ci_jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/code_standards.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/conda_for_dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/example_gallery.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29754 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/extending_fido.rst
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/funding.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.057222 sunpy-4.1.5/docs/dev_guide/contents/images/
--rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/images/actions_check_pr.png
--rw-r--r--   0 runner    (1001) docker     (123)    88979 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/images/actions_summary_check.png
--rw-r--r--   0 runner    (1001) docker     (123)    27285 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/images/checks.png
--rw-r--r--   0 runner    (1001) docker     (123)    59267 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/images/checks_pr.png
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/logger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/maintainer_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/map_rotate_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/new_objects.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/newcomers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/pr_checklist.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/pr_review_procedure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/public_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/remote_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/contents/units_quantities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/dev_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.057222 sunpy-4.1.5/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/diagrams/core_datatypes.dia
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/diagrams/map_class_hierarchy.dia
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/diagrams/package_layout.dia
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.057222 sunpy-4.1.5/docs/guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.061221 sunpy-4.1.5/docs/guide/acquiring_data/
--rw-r--r--   0 runner    (1001) docker     (123)    41831 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/acquiring_data/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/acquiring_data/fido.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/acquiring_data/hek.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/acquiring_data/helioviewer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/acquiring_data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35889 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/acquiring_data/jsoc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/acquiring_data/sample-data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/customization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.061221 sunpy-4.1.5/docs/guide/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/data_types/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27231 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/data_types/maps.rst
--rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/data_types/timeseries.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/logger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/ssw.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/tour.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/guide/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/nitpick-exceptions
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.061221 sunpy-4.1.5/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/0.8.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/0.9.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19714 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)    82435 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/1.1-wispr.png
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/2.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/2.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/3.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/3.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/4.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/4.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-20 17:01:58.000000 sunpy-4.1.5/docs/whatsnew/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.061221 sunpy-4.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.061221 sunpy-4.1.5/examples/acquiring_data/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/acquiring_data/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/acquiring_data/downloading_cutouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/acquiring_data/fido_metadata_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/acquiring_data/querying_the_GOES_event_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/acquiring_data/search_cdaweb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/acquiring_data/searching_vso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.065221 sunpy-4.1.5/examples/computer_vision_techniques/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/computer_vision_techniques/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/computer_vision_techniques/finding_masking_bright_pixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/computer_vision_techniques/loop_edge_enhance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/computer_vision_techniques/mask_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/computer_vision_techniques/off_limb_enhance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.065221 sunpy-4.1.5/examples/developer_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/developer_tools/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/developer_tools/remote_data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.065221 sunpy-4.1.5/examples/differential_rotation/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/differential_rotation/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/differential_rotation/comparing_rotation_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/differential_rotation/differentially_rotated_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/differential_rotation/differentially_rotated_gridlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/differential_rotation/reprojected_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.065221 sunpy-4.1.5/examples/example_template/
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/example_template/example_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.065221 sunpy-4.1.5/examples/map/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/brightness_pixel_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/compare_rotation_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/composite_map_AIA_HMI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/difference_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/hmi_contours_wcsaxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/image_bright_regions_gallery_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/map_contouring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/map_data_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/map_from_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/map_metadata_modification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/map_resampling_and_superpixels.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/map_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/map_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/plot_frameless_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map/submaps_and_cropping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.065221 sunpy-4.1.5/examples/map_transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/autoalign_aia_hmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/projection_custom_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/reprojection_aia_euvi_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/reprojection_align_aia_hmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/reprojection_carrington.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/reprojection_different_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/reprojection_spherical_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/map_transformations/upside_down_hmi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.069222 sunpy-4.1.5/examples/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/AIA_HMI_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/aia_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/arrayanimatorwcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/fading_between_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/finding_local_peaks_in_solar_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/finegrained_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/great_arc_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/grid_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/hmi_cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/hmi_synoptic_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/lat_lon_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/limb_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/lineAnimator_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/magnetogram_active_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/map_editcolormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/masked_composite_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/overplot_hek_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/plot_equator_prime_meridian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/plot_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/plotting_blank_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/quadrangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/rgb_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/simple_differential_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/solar_cycle_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/sunpy_matplotlib_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/three_map_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/wcsaxes_map_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/wcsaxes_plotting_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/plotting/xy_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.069222 sunpy-4.1.5/examples/saving_and_loading_data/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/saving_and_loading_data/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/saving_and_loading_data/coordinates_in_asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/saving_and_loading_data/genericmap_in_asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/saving_and_loading_data/genericmap_in_fits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.073222 sunpy-4.1.5/examples/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/goes_hek_m25.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/goes_xrs_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/power_spectra_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/timeseries_convolution_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/timeseries_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/timeseries_peak_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/time_series/timeseriesmetadata_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.073222 sunpy-4.1.5/examples/units_and_coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/AIA_limb_STEREO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/AltAz_Coordinate_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/STEREO_SECCHI_starfield.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/constants_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/getting_lasco_observer_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/getting_observer_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/map_slit_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/north_offset_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/parse_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/planet_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/radec_to_hpc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-20 17:01:58.000000 sunpy-4.1.5/examples/units_and_coordinates/venus_transit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.073222 sunpy-4.1.5/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-20 17:01:58.000000 sunpy-4.1.5/licenses/ASTROPY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-20 17:01:58.000000 sunpy-4.1.5/licenses/GLUE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 17:01:58.000000 sunpy-4.1.5/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-20 17:01:58.000000 sunpy-4.1.5/licenses/SCIKIT-LEARN.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 17:01:58.000000 sunpy-4.1.5/licenses/TOWNCRIER.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-20 17:01:58.000000 sunpy-4.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-04-20 17:02:32.137222 sunpy-4.1.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-04-20 17:01:58.000000 sunpy-4.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.073222 sunpy-4.1.5/sunpy/
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy/_compiler.c
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.077222 sunpy-4.1.5/sunpy/coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/frameattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    35194 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/metaframes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/offset_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/sun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.077222 sunpy-4.1.5/sunpy/coordinates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_frameattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_metaframes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_offset_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_sun.py
--rw-r--r--   0 runner    (1001) docker     (123)    46092 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50319 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/coordinates/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.077222 sunpy-4.1.5/sunpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.081222 sunpy-4.1.5/sunpy/data/data_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.081222 sunpy-4.1.5/sunpy/data/data_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/db_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/data_manager/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/sunpyrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.093222 sunpy-4.1.5/sunpy/data/test/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/20100621SRS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/2013_05_13__16_54_06_137__SOHO_LASCO_C3_white-light.jp2
--rw-r--r--   0 runner    (1001) docker     (123)    80880 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/20150101SRS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/20150306SRS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/20150906SRS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/20181209_180305_kcor_l2.header
--rw-r--r--   0 runner    (1001) docker     (123)    59987 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.093222 sunpy-4.1.5/sunpy/data/test/EIT/
--rw-r--r--   0 runner    (1001) docker     (123)   141120 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy/data/test/EIT/efz20040301.000010_s.fits
--rw-r--r--   0 runner    (1001) docker     (123)   141120 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT/efz20040301.010016_s.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.093222 sunpy-4.1.5/sunpy/data/test/EIT_header/
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.000010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.010016_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.020010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.030011_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.040010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.050010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.060010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.070014_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.080010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.090010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.100010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.110010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.120010_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/FGMG4_20110214_030443.7.header
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/HinodeSOT.header
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/HinodeXRT.header
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.093222 sunpy-4.1.5/sunpy/data/test/SWAP/
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/SWAP/resampled0_swap.header
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/SWAP/resampled1_swap.header
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/SWAP/resampled2_swap.header
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/SWAP/resampled3_swap.header
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/YohkohSXT.header
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/_generate_asdf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   149760 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/aia_171_level1.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/aiamap_genericmap_1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/annotation_ppt.db
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/cor1_20090615_000500_s4c1A.header
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header
--rw-r--r--   0 runner    (1001) docker     (123)    19358 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/euvi_20090615_000900_n4euA_s.header
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.093222 sunpy-4.1.5/sunpy/data/test/eve/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/eve/eve_01.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/eve/eve_02.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/eve/eve_03.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/eve/eve_04.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/eve/eve_05.txt
--rw-r--r--   0 runner    (1001) docker     (123)    89280 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits
--rw-r--r--   0 runner    (1001) docker     (123)    31680 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/gbm.fits
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/generated_sample.genx
--rw-r--r--   0 runner    (1001) docker     (123)   694080 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/go1520110607.fits
--rw-r--r--   0 runner    (1001) docker     (123)   219720 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/go1520120601.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    37737 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/goes_13_leap_second.nc
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/gzip_fits_test.file
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/gzip_test.fit.gz
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/gzip_test.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/gzip_test.fts.gz
--rw-r--r--   0 runner    (1001) docker     (123)   117097 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/heliographic_phase_map.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/hi_20110910_114721_s7h2A.header
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/hmi_synoptic.header
--rw-r--r--   0 runner    (1001) docker     (123)    95040 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/hsi_image_20101016_191218.fits
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/lasco_c2_25299383_s.header
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/lasco_c3.header
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/mdi_synoptic.header
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/observed-solar-cycle-indices-truncated.json
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/predicted-solar-cycle-truncated.json
--rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    89280 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/resampled_hmi.fits
--rw-r--r--   0 runner    (1001) docker     (123)    57333 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (123)    59635 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (123)    75990 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (123)    89560 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (123)   101102 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/seit_00171_fd_19961211_1900.header
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header
--rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)   369276 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/swap_lv1_20140606_000113.header
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/tca110810_truncated
--rw-r--r--   0 runner    (1001) docker     (123)   866179 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/test_ana.fz
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/tsi20010130_025823_a2.header
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.097222 sunpy-4.1.5/sunpy/data/test/waveunit/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/waveunit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/waveunit/mq130812.084253.header
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/waveunit/na120701.091058.header
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.097222 sunpy-4.1.5/sunpy/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/data/tests/test_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.097222 sunpy-4.1.5/sunpy/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    45842 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    32420 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.097222 sunpy-4.1.5/sunpy/database/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    35257 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tests/test_table.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24335 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/database/tests/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.097222 sunpy-4.1.5/sunpy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24738 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/appdirs_license.txt
--rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/distro.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/distro_license.rst
--rw-r--r--   0 runner    (1001) docker     (123)   102537 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/inflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/inflect_license.txt
--rw-r--r--   0 runner    (1001) docker     (123)    52276 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/extern/parse_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.097222 sunpy-4.1.5/sunpy/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/image/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/image/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/image/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/image/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/image/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/image/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/ana.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/cdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/file_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/jp2.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/io/special/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/io/special/asdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/io/special/asdf/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/converters/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/converters/generic_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/io/special/asdf/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/io/special/asdf/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.101222 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.105222 sunpy-4.1.5/sunpy/io/special/asdf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/tests/hgc_100.asdf
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/tests/test_coordinate_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/asdf/tests/test_genericmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/genx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/special/srs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.041221 sunpy-4.1.5/sunpy/io/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.105222 sunpy-4.1.5/sunpy/io/src/ana/
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/_pyana.c
--rw-r--r--   0 runner    (1001) docker     (123)    26833 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/anacompress.c
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/anacompress.h
--rw-r--r--   0 runner    (1001) docker     (123)    23203 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/anadecompress.c
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/anadecompress.h
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/anarw.c
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/anarw.h
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/src/ana/types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.105222 sunpy-4.1.5/sunpy/io/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/generate_genx.pro
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/test_ana.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/test_cdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/test_filetools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/test_genx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/test_jp2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/io/tests/test_srs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.105222 sunpy-4.1.5/sunpy/map/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/compositemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/header_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/map_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)   111957 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/mapbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/mapsequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/maputils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.109222 sunpy-4.1.5/sunpy/map/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/hinode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/mlso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/proba2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/psp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/rhessi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/sdo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/soho.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/solo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/source_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/suvi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.109222 sunpy-4.1.5/sunpy/map/sources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_aia_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_cor_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_eit_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_eui_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_euvi_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_hi_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_hmi_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_hmi_synoptic_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_iris_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_kcor_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_lasco_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_mdi_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_rhessi_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_sot_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_source_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_suvi_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_swap_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_sxt_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_trace_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_wispr_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/tests/test_xrt_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/sources/yohkoh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.113222 sunpy-4.1.5/sunpy/map/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_compositemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_header_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_map_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    63312 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_mapbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_mapsequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_maputils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/map/tests/test_reproject_to.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.113222 sunpy-4.1.5/sunpy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24205 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/base_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.113222 sunpy-4.1.5/sunpy/net/cdaweb/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/cdaweb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.113222 sunpy-4.1.5/sunpy/net/cdaweb/data/
--rw-r--r--   0 runner    (1001) docker     (123)   338383 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.113222 sunpy-4.1.5/sunpy/net/cdaweb/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/test/test_cdaweb.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/cdaweb/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.113222 sunpy-4.1.5/sunpy/net/dataretriever/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.113222 sunpy-4.1.5/sunpy/net/dataretriever/attrs/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/attrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/attrs/goes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/dataretriever/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/eve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/goes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/gong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/lyra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/norh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_eve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_goes_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_norh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/dataretriever/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/dataretriever/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20166 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/fido_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/hek/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek/hek.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/hek/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek/tests/test_hek.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/hek2vso/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek2vso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek2vso/hek2vso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/hek2vso/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek2vso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/hek2vso/tests/test_hek2vso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/helio/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/chaincode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/hec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.117222 sunpy-4.1.5/sunpy/net/helio/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/tests/test_chaincode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helio/tests/test_helio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/helioviewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/net/jsoc/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/net/jsoc/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43935 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)    38520 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/jsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/net/jsoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/jsoc/tests/test_jsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/net/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/test_attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/test_baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/test_fido.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/test_helioviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/tests/test_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/net/vso/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/net/vso/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/legacy_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/table_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/net/vso/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/tests/test_vso.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/vso.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/net/vso/zeep_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/physics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29915 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/physics/differential_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.121222 sunpy-4.1.5/sunpy/physics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/physics/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/physics/tests/reference/
--rw-r--r--   0 runner    (1001) docker     (123)    95355 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/physics/tests/reference/test_differential_rotation.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19734 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/physics/tests/test_differential_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/sun/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/sun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/sun/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/sun/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/sun/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/sun/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/sun/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/sun/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/figure_hashes_mpl_352_ft_261_astropy_51_animators_100.json
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/self_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/tests/test_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/tests/test_self_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/tests/tests/test_sunpy_data_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/time/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/time/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/tests/test_taiseconds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/tests/test_timerange.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/tests/test_utime.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/timeformats.py
--rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/time/timerange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.125222 sunpy-4.1.5/sunpy/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.129222 sunpy-4.1.5/sunpy/timeseries/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/eve.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/goes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/lyra.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/norh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.129222 sunpy-4.1.5/sunpy/timeseries/sources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/test_eve.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/test_fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/test_goes.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/test_lyra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/test_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/test_norh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/sources/tests/test_rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.129222 sunpy-4.1.5/sunpy/timeseries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/tests/test_timeseries_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/tests/test_timeseriesbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/tests/test_timeseriesmetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/timeseries_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    34725 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/timeseries/timeseriesbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.129222 sunpy-4.1.5/sunpy/util/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/datatype_factory_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/parfive_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.133222 sunpy-4.1.5/sunpy/util/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/sphinx/doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/sphinx/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.133222 sunpy-4.1.5/sunpy/util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_datatype_factory_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/tests/test_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/util/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.133222 sunpy-4.1.5/sunpy/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.133222 sunpy-4.1.5/sunpy/visualization/animator/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/animator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/animator/mapsequenceanimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.133222 sunpy-4.1.5/sunpy/visualization/animator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/animator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/animator/tests/test_mapsequenceanimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.133222 sunpy-4.1.5/sunpy/visualization/colormaps/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/color_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.137222 sunpy-4.1.5/sunpy/visualization/colormaps/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_dark_blue.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_dark_green.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_dark_red.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_yellow.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_171.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_195.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_284.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_304.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/grayscale.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/hi1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/hi2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/hmi_mag.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/idl_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/lasco_c2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/lasco_c3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/rhessi.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/std_gamma_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/stereo_cor1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/stereo_cor2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1216.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1550.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1600.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1700.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_171.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_195.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_284.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.137222 sunpy-4.1.5/sunpy/visualization/colormaps/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/colormaps/tests/test_cm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/limb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.137222 sunpy-4.1.5/sunpy/visualization/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/tests/test_drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-20 17:01:59.000000 sunpy-4.1.5/sunpy/visualization/wcsaxes_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 17:01:58.000000 sunpy-4.1.5/sunpy-dev-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:02:32.077222 sunpy-4.1.5/sunpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26626 2023-04-20 17:02:32.000000 sunpy-4.1.5/sunpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 17:02:31.000000 sunpy-4.1.5/sunpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-20 17:01:59.000000 sunpy-4.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.689846 sunpy-4.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (121)   211158 2022-11-04 18:23:42.000000 sunpy-4.1rc1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-11-04 18:23:42.000000 sunpy-4.1rc1/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-11-04 18:23:42.000000 sunpy-4.1rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-11-04 18:23:42.000000 sunpy-4.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4878 2022-11-04 18:24:17.689846 sunpy-4.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-11-04 18:23:42.000000 sunpy-4.1rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.621846 sunpy-4.1rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/about.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.621846 sunpy-4.1rc1/docs/code_ref/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.621846 sunpy-4.1rc1/docs/code_ref/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (121)     9899 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/coordinates/carrington.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14163 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/coordinates/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/coordinates/other_api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    19718 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/coordinates/rotatedsunframe.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6739 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/coordinates/velocities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/coordinates/wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/data.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/database.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/image.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4684 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/io.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/map.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/net.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/physics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/stability.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/sun.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/sunpy.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/sunpy_stability.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/time.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/timeseries.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/util.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/code_ref/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12821 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.621846 sunpy-4.1rc1/docs/dev_guide/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.625846 sunpy-4.1rc1/docs/dev_guide/contents/
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/backports.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3277 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/ci_jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11619 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/code_standards.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/conda_for_dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9582 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/example_gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    29752 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/extending_fido.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/funding.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.625846 sunpy-4.1rc1/docs/dev_guide/contents/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    47596 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/images/actions_check_pr.png
+-rw-r--r--   0 runner    (1001) docker     (121)    88979 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/images/actions_summary_check.png
+-rw-r--r--   0 runner    (1001) docker     (121)    27285 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/images/checks.png
+-rw-r--r--   0 runner    (1001) docker     (121)    59267 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/images/checks_pr.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3797 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/logger.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9916 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/maintainer_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/map_rotate_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3580 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/new_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14819 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/newcomers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/pr_checklist.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9767 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/pr_review_procedure.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/public_api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/remote_data.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12877 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/contents/units_quantities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/dev_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.625846 sunpy-4.1rc1/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (121)     5263 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/diagrams/core_datatypes.dia
+-rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/diagrams/map_class_hierarchy.dia
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/diagrams/package_layout.dia
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.625846 sunpy-4.1rc1/docs/guide/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.625846 sunpy-4.1rc1/docs/guide/acquiring_data/
+-rw-r--r--   0 runner    (1001) docker     (121)    41831 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/acquiring_data/database.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    30310 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/acquiring_data/fido.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13235 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/acquiring_data/hek.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/acquiring_data/helioviewer.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/acquiring_data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    35889 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/acquiring_data/jsoc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/acquiring_data/sample-data.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/customization.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.625846 sunpy-4.1rc1/docs/guide/data_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/data_types/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    27231 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/data_types/maps.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    32159 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/data_types/timeseries.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/logger.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9752 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/ssw.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9791 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/time.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14107 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/tour.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/guide/units.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/nitpick-exceptions
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (121)    10868 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/0.8.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6045 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/0.9.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    19713 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    82435 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/1.1-wispr.png
+-rw-r--r--   0 runner    (1001) docker     (121)    11396 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11729 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12432 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5651 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11238 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8181 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5335 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-11-04 18:23:42.000000 sunpy-4.1rc1/docs/whatsnew/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/acquiring_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/acquiring_data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/acquiring_data/downloading_cutouts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/acquiring_data/fido_metadata_queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/acquiring_data/querying_the_GOES_event_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/acquiring_data/search_cdaweb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/acquiring_data/searching_vso.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/computer_vision_techniques/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/computer_vision_techniques/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/computer_vision_techniques/finding_masking_bright_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/computer_vision_techniques/loop_edge_enhance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/computer_vision_techniques/mask_disk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/computer_vision_techniques/off_limb_enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/developer_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/developer_tools/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/developer_tools/remote_data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/differential_rotation/
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/differential_rotation/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/differential_rotation/comparing_rotation_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/differential_rotation/differentially_rotated_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/differential_rotation/differentially_rotated_gridlines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/differential_rotation/reprojected_map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/example_template/
+-rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/example_template/example_template.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/map/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/brightness_pixel_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/compare_rotation_results.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/composite_map_AIA_HMI.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/difference_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3934 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/hmi_contours_wcsaxes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/image_bright_regions_gallery_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/map_contouring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/map_data_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/map_from_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/map_metadata_modification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/map_resampling_and_superpixels.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/map_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/map_segment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/plot_frameless_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map/submaps_and_cropping.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.629846 sunpy-4.1rc1/examples/map_transformations/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/autoalign_aia_hmi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3595 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/projection_custom_origin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7628 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/reprojection_aia_euvi_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2961 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/reprojection_align_aia_hmi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/reprojection_carrington.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5401 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/reprojection_different_observers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/reprojection_spherical_screen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/map_transformations/upside_down_hmi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.633846 sunpy-4.1rc1/examples/plotting/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/aia_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3923 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/arrayanimatorwcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/fading_between_maps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3071 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/finding_local_peaks_in_solar_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2781 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/finegrained_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/great_arc_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/grid_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5019 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/hmi_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/hmi_synoptic_maps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/lat_lon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/limb_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/lineAnimator_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/magnetogram_active_regions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/map_editcolormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/overplot_hek_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/plot_equator_prime_meridian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/plot_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/plotting_blank_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/quadrangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3094 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/simple_differential_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/solar_cycle_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/sunpy_matplotlib_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/wcsaxes_map_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3802 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/wcsaxes_plotting_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/plotting/xy_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.633846 sunpy-4.1rc1/examples/saving_and_loading_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/saving_and_loading_data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/saving_and_loading_data/coordinates_in_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/saving_and_loading_data/genericmap_in_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/saving_and_loading_data/genericmap_in_fits.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.633846 sunpy-4.1rc1/examples/time_series/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/goes_hek_m25.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6062 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/goes_xrs_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/power_spectra_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/timeseries_convolution_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7546 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/timeseries_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/timeseries_peak_finding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/time_series/timeseriesmetadata_example.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.637846 sunpy-4.1rc1/examples/units_and_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (121)     3194 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/AIA_limb_STEREO.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/AltAz_Coordinate_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4979 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4837 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/STEREO_SECCHI_starfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/constants_reference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4469 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/getting_lasco_observer_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/getting_observer_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/map_slit_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/north_offset_frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3839 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/parse_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/planet_locations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8405 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/radec_to_hpc_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-11-04 18:23:42.000000 sunpy-4.1rc1/examples/units_and_coordinates/venus_transit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.637846 sunpy-4.1rc1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-11-04 18:23:42.000000 sunpy-4.1rc1/licenses/ASTROPY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-11-04 18:23:42.000000 sunpy-4.1rc1/licenses/GLUE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-04 18:23:42.000000 sunpy-4.1rc1/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-04 18:23:42.000000 sunpy-4.1rc1/licenses/SCIKIT-LEARN.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-11-04 18:23:42.000000 sunpy-4.1rc1/licenses/TOWNCRIER.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-11-04 18:23:42.000000 sunpy-4.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     6863 2022-11-04 18:24:17.689846 sunpy-4.1rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1132 2022-11-04 18:23:42.000000 sunpy-4.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.637846 sunpy-4.1rc1/sunpy/
+-rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy/_compiler.c
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.637846 sunpy-4.1rc1/sunpy/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15857 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/frameattributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35194 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/frames.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10357 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/metaframes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/offset_frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28071 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/sun.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.637846 sunpy-4.1rc1/sunpy/coordinates/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7089 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6549 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_frameattributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16571 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_frames.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11163 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_metaframes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_offset_frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24001 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_sun.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46093 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15902 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12870 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50297 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20368 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/coordinates/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.637846 sunpy-4.1rc1/sunpy/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8456 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.641846 sunpy-4.1rc1/sunpy/data/data_manager/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5307 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8002 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4751 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.641846 sunpy-4.1rc1/sunpy/data/data_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/tests/db_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7237 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/data_manager/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/sunpyrc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.649846 sunpy-4.1rc1/sunpy/data/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/20100621SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   484812 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/2013_05_13__16_54_06_137__SOHO_LASCO_C3_white-light.jp2
+-rw-r--r--   0 runner    (1001) docker     (121)  1077414 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/20150101SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/20150306SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/20150906SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11501 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/20181209_180305_kcor_l2.header
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.649846 sunpy-4.1rc1/sunpy/data/test/EIT/
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT/efz20040301.000010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   141120 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT/efz20040301.010016_s.fits
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.653846 sunpy-4.1rc1/sunpy/data/test/EIT_header/
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.000010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.010016_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.020010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.030011_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.040010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.050010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.060010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.070014_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.080010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.090010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.100010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.110010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.120010_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13283 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/FGMG4_20110214_030443.7.header
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/HinodeSOT.header
+-rw-r--r--   0 runner    (1001) docker     (121)     7246 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/HinodeXRT.header
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.653846 sunpy-4.1rc1/sunpy/data/test/SWAP/
+-rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/SWAP/resampled0_swap.header
+-rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/SWAP/resampled1_swap.header
+-rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/SWAP/resampled2_swap.header
+-rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/SWAP/resampled3_swap.header
+-rw-r--r--   0 runner    (1001) docker     (121)     9152 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/YohkohSXT.header
+-rw-r--r--   0 runner    (1001) docker     (121)     4591 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/_generate_asdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)   149760 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/aia_171_level1.fits
+-rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/aiamap_genericmap_1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/annotation_ppt.db
+-rw-r--r--   0 runner    (1001) docker     (121)    19763 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/cor1_20090615_000500_s4c1A.header
+-rw-r--r--   0 runner    (1001) docker     (121)     8747 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header
+-rw-r--r--   0 runner    (1001) docker     (121)    19358 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/euvi_20090615_000900_n4euA_s.header
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.653846 sunpy-4.1rc1/sunpy/data/test/eve/
+-rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/eve/eve_01.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/eve/eve_02.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/eve/eve_03.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/eve/eve_04.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/eve/eve_05.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    89280 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    31680 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/gbm.fits
+-rw-r--r--   0 runner    (1001) docker     (121)     7184 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/generated_sample.genx
+-rw-r--r--   0 runner    (1001) docker     (121)   694080 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/go1520110607.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   219720 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/go1520120601.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    37737 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/goes_13_leap_second.nc
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/gzip_test.fit.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/gzip_test.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/gzip_test.fts.gz
+-rw-r--r--   0 runner    (1001) docker     (121)   117097 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/heliographic_phase_map.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    20087 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/hi_20110910_114721_s7h2A.header
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/hmi_synoptic.header
+-rw-r--r--   0 runner    (1001) docker     (121)    95040 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/hsi_image_20101016_191218.fits
+-rw-r--r--   0 runner    (1001) docker     (121)     4877 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    12230 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header
+-rw-r--r--   0 runner    (1001) docker     (121)     6398 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/lasco_c2_25299383_s.header
+-rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/lasco_c3.header
+-rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     6641 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header
+-rw-r--r--   0 runner    (1001) docker     (121)     7451 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header
+-rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/mdi_synoptic.header
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/observed-solar-cycle-indices-truncated.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/predicted-solar-cycle-truncated.json
+-rw-r--r--   0 runner    (1001) docker     (121)    70003 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (121)    89280 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/resampled_hmi.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    57333 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (121)    59635 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (121)    75990 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (121)    89560 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (121)   101102 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (121)    17819 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header
+-rw-r--r--   0 runner    (1001) docker     (121)    32259 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf
+-rw-r--r--   0 runner    (1001) docker     (121)   369276 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf
+-rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/swap_lv1_20140606_000113.header
+-rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/tca110810_truncated
+-rw-r--r--   0 runner    (1001) docker     (121)   866179 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/test_ana.fz
+-rw-r--r--   0 runner    (1001) docker     (121)     5426 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/tsi20010130_025823_a2.header
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.653846 sunpy-4.1rc1/sunpy/data/test/waveunit/
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/waveunit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header
+-rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/waveunit/mq130812.084253.header
+-rw-r--r--   0 runner    (1001) docker     (121)     3239 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/waveunit/na120701.091058.header
+-rw-r--r--   0 runner    (1001) docker     (121)     7370 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.653846 sunpy-4.1rc1/sunpy/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/data/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.653846 sunpy-4.1rc1/sunpy/database/
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8957 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13123 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45842 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32456 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.653846 sunpy-4.1rc1/sunpy/database/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19520 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8473 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35195 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tests/test_table.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    24343 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/database/tests/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/extern/
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24738 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/appdirs_license.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    49330 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/distro.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11324 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/distro_license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)   102537 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/inflect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/inflect_license.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    52276 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/extern/parse_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/image/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7952 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/image/resample.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/image/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/image/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/image/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13876 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/image/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19012 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/image/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/io/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12275 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/_fits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/ana.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8855 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8017 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/file_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4612 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/jp2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/io/special/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/io/special/asdf/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/io/special/asdf/converters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/converters/frames.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/converters/generic_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/entry_points.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/io/special/asdf/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.657846 sunpy-4.1rc1/sunpy/io/special/asdf/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.661846 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.661846 sunpy-4.1rc1/sunpy/io/special/asdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/tests/hgc_100.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/tests/test_coordinate_frames.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/asdf/tests/test_genericmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10122 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/genx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6944 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/special/srs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.601846 sunpy-4.1rc1/sunpy/io/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.661846 sunpy-4.1rc1/sunpy/io/src/ana/
+-rw-r--r--   0 runner    (1001) docker     (121)    11567 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/_pyana.c
+-rw-r--r--   0 runner    (1001) docker     (121)    26833 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/anacompress.c
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/anacompress.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23203 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/anadecompress.c
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/anadecompress.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11924 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/anarw.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/anarw.h
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/src/ana/types.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.661846 sunpy-4.1rc1/sunpy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5746 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/generate_genx.pro
+-rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/test_ana.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/test_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/test_filetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6711 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5078 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/test_genx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/test_jp2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/io/tests/test_srs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.665846 sunpy-4.1rc1/sunpy/map/
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/_units.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18571 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/compositemap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18098 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/header_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14054 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)   111356 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/mapbase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21213 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/mapsequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17396 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/maputils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.665846 sunpy-4.1rc1/sunpy/map/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6988 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/hinode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/iris.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3223 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/mlso.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/proba2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/psp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3452 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/rhessi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8004 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/sdo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10885 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/soho.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/solo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/source_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4896 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/stereo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4654 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/suvi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.665846 sunpy-4.1rc1/sunpy/map/sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_aia_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_cor_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_eit_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_eui_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_euvi_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_hi_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_hmi_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_hmi_synoptic_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_iris_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_kcor_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_lasco_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_mdi_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_rhessi_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_sot_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_suvi_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_swap_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_sxt_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_trace_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11450 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_wispr_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/tests/test_xrt_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/trace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/sources/yohkoh.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/map/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4401 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4782 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_compositemap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9960 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_header_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11770 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60478 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_mapbase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9018 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_mapsequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13171 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_maputils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5003 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/map/tests/test_reproject_to.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/net/
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8896 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24205 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/attr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16511 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/base_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/net/cdaweb/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6694 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/cdaweb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/net/cdaweb/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   316041 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4574 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/net/cdaweb/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/test/test_cdaweb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      857 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/cdaweb/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/net/dataretriever/
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/net/dataretriever/attrs/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/attrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/attrs/goes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11360 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.669846 sunpy-4.1rc1/sunpy/net/dataretriever/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/eve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15708 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/goes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/gong.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/lyra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7291 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/noaa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3707 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/norh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9053 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5646 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_eve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8990 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7996 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_goes_ud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3193 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4290 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9392 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6358 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_norh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8880 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/dataretriever/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/dataretriever/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19923 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/fido_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/hek/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17902 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7273 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek/hek.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/hek/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6484 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek/tests/test_hek.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/hek2vso/
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek2vso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7767 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek2vso/hek2vso.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/hek2vso/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek2vso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/hek2vso/tests/test_hek2vso.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/helio/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/chaincode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9043 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/hec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7691 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/helio/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/tests/test_chaincode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10541 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helio/tests/test_helio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17388 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/helioviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/jsoc/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7160 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/jsoc/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43936 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (121)    38219 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/jsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/jsoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13201 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/jsoc/tests/test_jsoc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19724 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.673846 sunpy-4.1rc1/sunpy/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11128 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/test_attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/test_baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15589 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/test_fido.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6006 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/test_helioviewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13551 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/tests/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/net/vso/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6173 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/net/vso/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20482 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/legacy_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5041 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/table_response.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/net/vso/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6680 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12233 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/tests/test_vso.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26017 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/vso.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/net/vso/zeep_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/physics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30166 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/physics/differential_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/physics/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/physics/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/physics/tests/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)    95355 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/physics/tests/reference/test_differential_rotation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20466 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/physics/tests/test_differential_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/sun/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/sun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9845 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/sun/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/sun/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/sun/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/sun/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/sun/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/sun/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9162 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/figure_hashes_mpl_352_ft_261_astropy_51_animators_100.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9162 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7339 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2462 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/self_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/tests/test_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/tests/test_self_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/tests/tests/test_sunpy_data_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/time/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.677846 sunpy-4.1rc1/sunpy/time/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/tests/test_taiseconds.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10110 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8881 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/tests/test_timerange.py
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/tests/test_utime.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12463 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/timeformats.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14424 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/time/timerange.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.681846 sunpy-4.1rc1/sunpy/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28761 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.681846 sunpy-4.1rc1/sunpy/timeseries/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14296 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/eve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9176 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13462 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/goes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7666 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/lyra.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13108 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/noaa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6163 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/norh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8196 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.681846 sunpy-4.1rc1/sunpy/timeseries/sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_eve.py
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_goes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_lyra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_norh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.681846 sunpy-4.1rc1/sunpy/timeseries/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18317 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/tests/test_timeseries_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23326 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/tests/test_timeseriesbase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21538 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/tests/test_timeseriesmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19718 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/timeseries_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34723 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/timeseries/timeseriesbase.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.681846 sunpy-4.1rc1/sunpy/util/
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7263 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5990 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/datatype_factory_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15164 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/functools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3330 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7649 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6514 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/net.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/parfive_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.681846 sunpy-4.1rc1/sunpy/util/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/sphinx/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/sphinx/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.685846 sunpy-4.1rc1/sunpy/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7062 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4566 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_datatype_factory_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15999 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_net.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5078 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8198 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/tests/test_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/util/xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.685846 sunpy-4.1rc1/sunpy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.685846 sunpy-4.1rc1/sunpy/visualization/animator/
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/animator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/animator/mapsequenceanimator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.685846 sunpy-4.1rc1/sunpy/visualization/animator/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/animator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/animator/tests/test_mapsequenceanimator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.685846 sunpy-4.1rc1/sunpy/visualization/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7609 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/cm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12309 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/color_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.685846 sunpy-4.1rc1/sunpy/visualization/colormaps/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_dark_blue.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_dark_green.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_dark_red.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_yellow.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_171.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_195.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_284.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_304.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/grayscale.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/hi1.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/hi2.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/hmi_mag.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/idl_3.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/lasco_c2.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/lasco_c3.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/rhessi.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/std_gamma_2.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/stereo_cor1.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/stereo_cor2.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1216.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1550.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1600.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1700.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_171.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_195.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_284.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.689846 sunpy-4.1rc1/sunpy/visualization/colormaps/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/colormaps/tests/test_cm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10258 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/limb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.689846 sunpy-4.1rc1/sunpy/visualization/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/tests/test_drawing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy/visualization/wcsaxes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-11-04 18:23:42.000000 sunpy-4.1rc1/sunpy-dev-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:24:17.637846 sunpy-4.1rc1/sunpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4878 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    26264 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-04 18:24:17.000000 sunpy-4.1rc1/sunpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-11-04 18:23:42.000000 sunpy-4.1rc1/tox.ini
```

### Comparing `sunpy-4.1.5/CHANGELOG.rst` & `sunpy-4.1rc1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,319 +1,7 @@
-4.1.5 (2023-04-20)
-==================
-
-New Features
-------------
-
-- Able to download files from REST/TAP Data Providers from the VSO. (`#6887 <https://github.com/sunpy/sunpy/pull/6887>`__)
-
-
-Bug Fixes
----------
-
-- Pass in "max_splits" to Parfive to prevent multi connections to JSOC for JSOC only queries. (`#6921 <https://github.com/sunpy/sunpy/pull/6921>`__)
-
-
-Documentation
--------------
-
-- Added clarifying detail (in the `~sunpy.time.TimeUTime` docstring) for how the ``utime`` time format handles seconds on a day with a leap second. (`#6894 <https://github.com/sunpy/sunpy/pull/6894>`__)
-
-
-4.1.4 (2023-03-31)
-==================
-
-Bug Fixes
----------
-
-- When using ``autoalign=True`` when plotting maps, the result was misaligned by half a pixel. (`#6796 <https://github.com/sunpy/sunpy/pull/6796>`__)
-- :meth:`sunpy.map.GenericMap.submap` can now handle a '~astropy.coordinates.BaseCoordinateFrame' as input. (`#6820 <https://github.com/sunpy/sunpy/pull/6820>`__)
-
-
-Documentation
--------------
-
-- Added a note in examples :ref:`sphx_glr_generated_gallery_map_transformations_autoalign_aia_hmi.py` and :ref:`sphx_glr_generated_gallery_map_transformations_reprojection_align_aia_hmi.py` suggesting to use :meth:`~sunpy.coordinates.Helioprojective.assume_spherical_screen` to retain off-disk HMI data. (`#6855 <https://github.com/sunpy/sunpy/pull/6855>`__)
-
-
-4.1.3 (2023-02-14)
-==================
-
-Breaking Changes
-----------------
-
-- `~sunpy.net.dataretriever.XRSClient` now provides the re-processed GOES-XRS 8-15 data from NOAA.
-  These files are now all NetCDF and not FITS files. (`#6737 <https://github.com/sunpy/sunpy/pull/6737>`__)
-
-
-New Features
-------------
-
-- `~sunpy.net.dataretriever.SUVIClient` now provides GOES-18 SUVI data. (`#6737 <https://github.com/sunpy/sunpy/pull/6737>`__)
-
-
-Bug Fixes
----------
-
-- Fixed a bug that prevented specifying a `~astropy.coordinates.BaseCoordinateFrame` (as opposed to a `~astropy.coordinates.SkyCoord`) to :meth:`sunpy.map.GenericMap.draw_quadrangle`. (`#6648 <https://github.com/sunpy/sunpy/pull/6648>`__)
-- HMI JPEG2000 files from Helioviewer could not be loaded due to a bug in setting the plotting normalization.
-  This has been fixed. (`#6710 <https://github.com/sunpy/sunpy/pull/6710>`__)
-- The ``data_manager`` was not raising failed downloads correctly and would continue as if the file existed locally.
-  Now it will raise any errors from ``parfive``. (`#6711 <https://github.com/sunpy/sunpy/pull/6711>`__)
-- `~sunpy.map.sources.XRTMap` will now set the unit for XRT files if the ``BUNIT`` key is missing. (`#6725 <https://github.com/sunpy/sunpy/pull/6725>`__)
-- `~sunpy.net.dataretriever.XRSClient` update use the new url for which the GOES-XRS 8-15 data is provided by NOAA. (`#6737 <https://github.com/sunpy/sunpy/pull/6737>`__)
-- Updated `~sunpy.database` to be compatible with ``SQLAlchemy`` versions >=2.0 (`#6749 <https://github.com/sunpy/sunpy/pull/6749>`__)
-
-
-4.1.2 (2023-01-27)
-==================
-
-New Features
-------------
-
-- Able to detect gzip-compressed FITS files even if they don't have the ``.gz`` extension in the filename.
-  `~sunpy.io.detect_filetype` now looks for the right file signature while checking
-  for gzipped FITS files. (`#6693 <https://github.com/sunpy/sunpy/pull/6693>`__)
-
-
-Internal Changes
-----------------
-
-- The current version of ``SQLAlchemy`` has been fixed to be <2.0 until we have ensured that the current database module works with it. (`#6694 <https://github.com/sunpy/sunpy/pull/6694>`__)
-
-
-4.1.1 (2022-12-30)
-==================
-
-New Features
-------------
-
-- Added three tutorials which replicate `~sunpy.map.CompositeMap` functionality (:ref:`sphx_glr_generated_gallery_plotting_AIA_HMI_composite.py`, :ref:`sphx_glr_generated_gallery_plotting_masked_composite_plot.py`, :ref:`sphx_glr_generated_gallery_plotting_three_map_composite.py`).
-  A fourth tutorial (:ref:`sphx_glr_generated_gallery_plotting_rgb_composite.py`) demonstrates how to create an RGB image with three different maps. (`#6459 <https://github.com/sunpy/sunpy/pull/6459>`__)
-
-
-Bug Fixes
----------
-
-- Fixed the incorrect calculation in :func:`~sunpy.map.header_helper.make_fitswcs_header` of the rotation matrix from a rotation angle when the pixels are non-square. (`#6597 <https://github.com/sunpy/sunpy/pull/6597>`__)
-- Fixed an issue with loading old EIT fits files with `sunpy.map.Map` where the date could not be parsed. (`#6605 <https://github.com/sunpy/sunpy/pull/6605>`__)
-
-
-Documentation
--------------
-
-- Added `sunpy.map.PixelPair` to the reference documentation. (`#6620 <https://github.com/sunpy/sunpy/pull/6620>`__)
-
-
-4.1.0 (2022-11-11)
-==================
-
-Breaking Changes
-----------------
-
-- Updated the sample data file, ``AIA_171_ROLL_IMAGE`` to be rice compressed instead of gzip compressed.
-  This means that the data is now stored in the second HDU. (`#6221 <https://github.com/sunpy/sunpy/pull/6221>`__)
-
-
-Deprecations
-------------
-
-- Passing positional arguments to all ``timeseries`` ``peek()`` methods
-  is now deprecated, and will raise an error in sunpy 5.1. Pass the arguments
-  with keywords (e.g. ``title='my plot title'``) instead. (`#6310 <https://github.com/sunpy/sunpy/pull/6310>`__)
-- Using `sunpy.timeseries.GenericTimeSeries.index` is deprecated.
-  Use `~sunpy.timeseries.GenericTimeSeries.time` to get an astropy Time object,
-  or ``ts.to_dataframe().index`` to get the times as a pandas ``DataTimeIndex``. (`#6327 <https://github.com/sunpy/sunpy/pull/6327>`__)
-- Deprecated the ``sunpy.visualization.limb`` module.
-  The ``sunpy.visualization.limb.draw_limb`` function has been moved into
-  `~sunpy.visualization.drawing` as :func:`~sunpy.visualization.drawing.limb`. (`#6332 <https://github.com/sunpy/sunpy/pull/6332>`__)
-- The ``sunpy.net.helioviewer`` module is deprecated and will be removed in version 5.1.
-  The Helioviewer Project now maintains a replacement Python library called `hvpy <https://hvpy.readthedocs.io/en/latest/>`__.
-  As such, in consultation with the Helioviewer Project, we have decided to deprecate the ``HelioviewerClient`` class. (`#6404 <https://github.com/sunpy/sunpy/pull/6404>`__)
-- Passing the ``algorithm``, ``return_footprint`` arguments as positional arguments is deprecated. Pass them as keyword arguments (e.g. ``..., return_footprint=True, ...``) instead. (`#6406 <https://github.com/sunpy/sunpy/pull/6406>`__)
-- :func:`sunpy.data.download_sample_data` is now deprecated.
-  Use :func:`sunpy.data.sample.download_all` instead. (`#6426 <https://github.com/sunpy/sunpy/pull/6426>`__)
-- The sunpy.database module is no longer actively maintained and has a number of outstanding issues.
-  It is anticiapted that sunpy.database will be formally deprecated in sunpy 5.0 and removed in sunpy 6.0.
-  If you are using sunpy.database and would like to see a replacement, please join the discussion thread at https://community.openastronomy.org/t/deprecating-sunpy-database/495. (`#6498 <https://github.com/sunpy/sunpy/pull/6498>`__)
-
-
-Removals
---------
-
-- The ``sunpy.io.fits`` sub-module has been removed, as it was designed for internal use.
-  Use the `astropy.io.fits` module instead for more generic functionality to read FITS files. (`#6432 <https://github.com/sunpy/sunpy/pull/6432>`__)
-- The ``sunpy.physics.solar_rotation`` sub-module has been removed, having been moved to `sunkit_image.coalignment`. (`#6433 <https://github.com/sunpy/sunpy/pull/6433>`__)
-- Most of the `sunpy.visualization.animator` subpackage has been removed, with the exception of `~sunpy.visualization.animator.MapSequenceAnimator`
-  It has been moved into the standalone `mpl-animators <https://pypi.org/project/mpl-animators>`_ package
-  Please update your imports to replace ``sunpy.visualization.animator`` with ``mpl_animators``. (`#6434 <https://github.com/sunpy/sunpy/pull/6434>`__)
-- Remove ``GenericMap.shift`` method and the ``GenericMap.shifted_value``.
-  Use `~sunpy.map.GenericMap.shift_reference_coord` instead. (`#6437 <https://github.com/sunpy/sunpy/pull/6437>`__)
-- ``sunpy.util.scraper`` has been removed. Use `sunpy.net.scraper` instead. (`#6438 <https://github.com/sunpy/sunpy/pull/6438>`__)
-- ``sunpy.image.coalignment`` has been removed. Use `sunkit_image.coalignment` instead, which contains all the same functionality. (`#6440 <https://github.com/sunpy/sunpy/pull/6440>`__)
-- :meth:`sunpy.map.GenericMap.draw_limb` can no longer be used to draw the limb on a non-WCS Axes plot. (`#6533 <https://github.com/sunpy/sunpy/pull/6533>`__)
-- :meth:`sunpy.image.resample` no longer accepts "neighbour" as an interpolation method.
-  Use "nearest" instead. (`#6537 <https://github.com/sunpy/sunpy/pull/6537>`__)
-- :meth:`sunpy.image.transform.affine_transform` and :func:`sunpy.map.GenericMap.rotate` no longer accepts the ``use_scipy`` keyword. (`#6538 <https://github.com/sunpy/sunpy/pull/6538>`__)
-
-
-New Features
-------------
-
-- Updated and expanded the HTML representation for `~sunpy.timeseries.TimeSeries`. (`#5951 <https://github.com/sunpy/sunpy/pull/5951>`__)
-- When reading CDF files, any columns with a floating point data type now have their masked values converted to NaN. (`#5956 <https://github.com/sunpy/sunpy/pull/5956>`__)
-- Add support for saving `~sunpy.map.GenericMap` as JPEG 2000 files. (`#6153 <https://github.com/sunpy/sunpy/pull/6153>`__)
-- Add a function `sunpy.map.extract_along_coord` that, for a given set of coordinates,
-  finds each array index that crosses the line traced by those coordinates and returns the value of the data
-  array of a given map at those array indices. (`#6189 <https://github.com/sunpy/sunpy/pull/6189>`__)
-- Three new maps have been added to the sample data from STEREO A and STEREO B at
-  195 Angstrom, and AIA at 193 Angstrom. These images are from a time when
-  the three spacecraft were equally spaced around the Sun, and therefore form
-  near complete instantaneous coverage of the solar surface.
-
-  Users upgrading to this version will find this three files download when they
-  use the sample data for the first time. (`#6197 <https://github.com/sunpy/sunpy/pull/6197>`__)
-- Added a SDO/AIA 1600 file of the Venus transit to the sunpy sample data. (`#6242 <https://github.com/sunpy/sunpy/pull/6242>`__)
-- Created the `sunpy.visualization.drawing` module which includes
-  new :func:`~sunpy.visualization.drawing.equator` and
-  :func:`~sunpy.visualization.drawing.prime_meridian` functions. (`#6251 <https://github.com/sunpy/sunpy/pull/6251>`__)
-- Expose GOES quality flags in order to allow filtering corrupt values when using the `~sunpy.timeseries.sources.goes.XRSTimeSeries`. (`#6260 <https://github.com/sunpy/sunpy/pull/6260>`__)
-- All TimeSeries plotting methods now consistently set the same
-  formatter and locator for the x-axis. (`#6264 <https://github.com/sunpy/sunpy/pull/6264>`__)
-- :meth:`sunpy.timeseries.GenericTimeSeries.peek` now takes a ``title`` argument
-  to set the title of the plot. (`#6304 <https://github.com/sunpy/sunpy/pull/6304>`__)
-- Added the `sunpy.timeseries.GenericTimeSeries.time` property to get the times
-  of a timeseries as a `~astropy.time.Time` object. (`#6327 <https://github.com/sunpy/sunpy/pull/6327>`__)
-- Added the :ref:`sphx_glr_generated_gallery_plotting_plot_equator_prime_meridian.py` example to the Example Gallery. (`#6332 <https://github.com/sunpy/sunpy/pull/6332>`__)
-- Added a new function :func:`sunpy.map.header_helper.make_heliographic_header` to help with generating FITS-WCS headers in Carrington or Stonyhurst coordinate systems that span the entire solar surface. (`#6415 <https://github.com/sunpy/sunpy/pull/6415>`__)
-- Sample data files provided through `sunpy.data.sample` are now downloaded individually on demand rather than being all downloaded upon import of that module.
-  To download all sample data files, call :func:`sunpy.data.sample.download_all`. (`#6426 <https://github.com/sunpy/sunpy/pull/6426>`__)
-- `~.XRSTimeSeries` is now able to parse the primary detector information from the GOES-R XRS data if available. (`#6454 <https://github.com/sunpy/sunpy/pull/6454>`__)
-- `sunpy.net.Scraper` now includes treats files as spanning a full interval equal to the smallest increment specified in the file pattern.
-  For example, a pattern like ``"%Y.txt"`` that only contains a year specifier will be considered to span that full year.
-
-  This means searches that fall entirely within the whole interval spanned by a pattern will return that file, where previously they did not.
-  As an example, matching ``"%Y.txt"`` with ``TimeRange('2022-02-01', '2022-04-01')`` will now return ``["2022.txt"]`` where previously no files were returned. (`#6472 <https://github.com/sunpy/sunpy/pull/6472>`__)
-- Implemented site configuration for sunpyrc, and modified documentation for sunpy customization. (`#6478 <https://github.com/sunpy/sunpy/pull/6478>`__)
-- :func:`~sunpy.map.header_helper.make_fitswcs_header` now includes the keyword argument ``unit`` for setting the
-  ``BUNIT`` FITS keyword in the resulting header.
-  This will take precedence over any unit information attached to ``data``. (`#6499 <https://github.com/sunpy/sunpy/pull/6499>`__)
-- If the ``data`` argument to :func:`~sunpy.map.header_helper.make_fitswcs_header` is an `~astropy.units.Quantity`,
-  the associated unit will be used to set the ``BUNIT`` FITS keyword in the resulting header. (`#6499 <https://github.com/sunpy/sunpy/pull/6499>`__)
-- Added a 304 sample data file called ``AIA_304_IMAGE``. (`#6546 <https://github.com/sunpy/sunpy/pull/6546>`__)
-
-
-Bug Fixes
----------
-
-- Fix a bug that prevented EUI maps with missing wavelength metadata loading. (`#6199 <https://github.com/sunpy/sunpy/pull/6199>`__)
-- The `sunpy.net.dataretriever.sources.noaa.SRSClient` was not correctly setting the passive mode for FTP connection resulting in a permission error.
-  This has been fixed. (`#6256 <https://github.com/sunpy/sunpy/pull/6256>`__)
-- Fixed `~sunpy.timeseries.sources.XRSTimeSeries` inability to read leap-second files for GOES.
-  It floors the leap-second timestamp to be ``59.999``, so that Python datetime does not raise an exception. (`#6262 <https://github.com/sunpy/sunpy/pull/6262>`__)
-- Changed the default scaling for `~sunpy.map.sources.EUIMap` from a linear stretch to a asinh stretch.
-
-  To revert to the previous linear stretch do the following::
-
-       from astropy.visualization import ImageNormalize, LinearStretch
-       euimap.plot_settings["norm"] = ImageNormalize(stretch=LinearStretch()) (`#6285 <https://github.com/sunpy/sunpy/pull/6285>`__)
-- Fixed bugs when working with a coordinate frame where the observer is specified in `~sunpy.coordinates.frames.HeliographicStonyhurst` with a Cartesian representation, which is equivalent to Heliocentric Earth Equatorial (HEEQ).
-  Now, the observer will always be converted to spherical representation when the coordinate frame is created. (`#6311 <https://github.com/sunpy/sunpy/pull/6311>`__)
-- Fixed an error when Fido returns zero results from the VSO
-  and some results from at least one other data source. This
-  (now fixed) error is only present when using numpy version >= 1.23. (`#6318 <https://github.com/sunpy/sunpy/pull/6318>`__)
-- If a level 1 XRT file does not specify the heliographic longitude of the spacecraft,
-  a silent assumption is made that the spacecraft is at zero Stonyhurst
-  heliographic longitude (i.e., the same longitude as Earth). (`#6333 <https://github.com/sunpy/sunpy/pull/6333>`__)
-- The sample data retry was failing under parfive 2.0.0. (`#6334 <https://github.com/sunpy/sunpy/pull/6334>`__)
-- Fixed bug that prevented `~sunpy.coordinates.metaframes.RotatedSunFrame` instances from being pickled. (`#6342 <https://github.com/sunpy/sunpy/pull/6342>`__)
-- Fix a bug in loading `.XRSTimeSeries` due to unsupported quality flag column names. (`#6410 <https://github.com/sunpy/sunpy/pull/6410>`__)
-- Adds units (dimensionless units) to the quality columns in `.XRSTimeSeries`. (`#6423 <https://github.com/sunpy/sunpy/pull/6423>`__)
-- Refactored `~sunpy.map.sources.SXTMap` to use ITRS observer coordinate information
-  in header rather than incorrect HGS keywords.
-  The `~sunpy.map.sources.SXTMap` also now uses the default ``dsun`` property as this
-  information can be derived from the (now corrected) observer coordinate. (`#6436 <https://github.com/sunpy/sunpy/pull/6436>`__)
-- In `sunpy.map.GenericMap.coordinate_system` and `sunpy.map.GenericMap.date`, the default values
-  will now be used if the expected key(s) used to derive those properties are empty.
-  Previously, empty values of these keys were not treated as missing and thus the default values
-  were not correctly filled in. (`#6436 <https://github.com/sunpy/sunpy/pull/6436>`__)
-- Fixed a bug where the observer coordinate was incorrectly determined for `~sunpy.map.sources.KCorMap`. (`#6447 <https://github.com/sunpy/sunpy/pull/6447>`__)
-- Trying to download an empty search response from the JSOC now results in an empty results object.
-  Previously the results object contained the path to the sunpy download directory. (`#6449 <https://github.com/sunpy/sunpy/pull/6449>`__)
-- Removed an error when searching CDAWEB using `sunpy.net.Fido` and no results are returned.
-  An empty response table is now returned. (`#6450 <https://github.com/sunpy/sunpy/pull/6450>`__)
-- Fix a bug to parse the GOES "observatory" number in `~.XRSTimeSeries` for GOES 13, 14, 15 and for the 1 minute GOES-R data. (`#6451 <https://github.com/sunpy/sunpy/pull/6451>`__)
-- Changed the default scaling for `~sunpy.map.sources.XRTMap` from a linear stretch to `~astropy.visualization.LogStretch`.
-
-  To revert to the previous linear stretch do the following::
-
-       from astropy.visualization import ImageNormalize, LinearStretch
-       xrtmap.plot_settings["norm"] = ImageNormalize(stretch=LinearStretch()) (`#6480 <https://github.com/sunpy/sunpy/pull/6480>`__)
-- Fix the ``detector`` property of `~sunpy.map.sources.SOTMap` to return "SOT". (`#6480 <https://github.com/sunpy/sunpy/pull/6480>`__)
-- The right-hand y-axis of the GOES-XRS timeseries plots with labelled flare classes
-  now automatically scales with the left-hand y-axis. (`#6486 <https://github.com/sunpy/sunpy/pull/6486>`__)
-- Add support for Python 3.11.
-
-  The deprecated `cgi.parse_header` is now available as
-  `sunpy.util.net.parse_header`. (`#6512 <https://github.com/sunpy/sunpy/pull/6512>`__)
-- Fixed the metadata handling of :meth:`~sunpy.map.GenericMap.resample` and :meth:`~sunpy.map.GenericMap.superpixel` so that the CDELTi values are scaled and the PCi_j matrix (if used) is modified in the correct manner for asymmetric scaling.
-  The previous approach of having the PCi_j matrix store all of the scaling resulted in non-intuitive behaviors when accessing the `~sunpy.map.GenericMap.scale` and `~sunpy.map.GenericMap.rotation_matrix` properties, and when de-rotating a map via :meth:`~sunpy.map.GenericMap.rotate`. (`#6571 <https://github.com/sunpy/sunpy/pull/6571>`__)
-- Fixd a bug with the `sunpy.map.GenericMap.scale` property for maps containing only the CDij matrix where the scale was not being determined from the CDij matrix. (`#6573 <https://github.com/sunpy/sunpy/pull/6573>`__)
-- Fixed a bug with the `sunpy.map.GenericMap.rotation_matrix` property for maps using the CDij matrix formulism where the rotation matrix would be calculated incorrectly for non-square pixels. (`#6573 <https://github.com/sunpy/sunpy/pull/6573>`__)
-- Fixed a bug where :func:`~sunpy.time.parse_time` would always disregard the remainder of a time string starting with the final period if it was followed by only zeros, which could affect the parsing of the time string. (`#6581 <https://github.com/sunpy/sunpy/pull/6581>`__)
-
-
-Documentation
--------------
-
-- Improved annotations in the SRS active regions plotting example. (`#6196 <https://github.com/sunpy/sunpy/pull/6196>`__)
-- Updated gallery examples that use STEREO data to use sample data instead
-  of searching for and downloading data via Fido. (`#6197 <https://github.com/sunpy/sunpy/pull/6197>`__)
-- Added the current bugfix release policy to the docs. (`#6336 <https://github.com/sunpy/sunpy/pull/6336>`__)
-- The :ref:`map_guide` and :ref:`timeseries_guide` have been reviewed and updated. (`#6345 <https://github.com/sunpy/sunpy/pull/6345>`__)
-- Adds a pull request check list to the Developer's Guide. (`#6346 <https://github.com/sunpy/sunpy/pull/6346>`__)
-- Improved the plotting guide. (`#6430 <https://github.com/sunpy/sunpy/pull/6430>`__)
-- Slight improvements to the downloading data with Fido part of the guide. (`#6444 <https://github.com/sunpy/sunpy/pull/6444>`__)
-- Split the units and coordinate guides on to separate pages, and made minor improvements to them. (`#6462 <https://github.com/sunpy/sunpy/pull/6462>`__)
-- Added a how-to guide (``conda_for_dependencies``) for using ``conda`` to set up an environment with the complete set of dependencies to use all optional features, build the documentation, and/or run the full test suite.
-  The guide also describes how best to have an editable installation of ``sunpy`` in this environment. (`#6524 <https://github.com/sunpy/sunpy/pull/6524>`__)
-
-
-Internal Changes
-----------------
-
-- Added a ``columns`` keyword to each plot method for all `sunpy.timeseries.GenericTimeSeries` sources. (`#6056 <https://github.com/sunpy/sunpy/pull/6056>`__)
-- Added a script in the ``sunpy/tools`` that will update all the Python libraries in ``sunpy/extern``. (`#6127 <https://github.com/sunpy/sunpy/pull/6127>`__)
-- Added automatic conversion of unit strings in CDF files to astropy unit objects for the following instruments: PSP/ISOIS, SOHO/CELIAS, SOHO/COSTEP-EPHIN, and SOHO/ERNE. (`#6159 <https://github.com/sunpy/sunpy/pull/6159>`__)
-- Add an environment variable ``SUNPY_NO_BUILD_ANA_EXTENSION`` which when present
-  will cause sunpy to not compile the ANA C extension when building from source. (`#6166 <https://github.com/sunpy/sunpy/pull/6166>`__)
-- ``sunpy`` now uses the `Limited Python API <https://docs.python.org/3/c-api/stable.html>`__.
-  Therefore, one binary distribution (wheel) per platform is now published and it is compatible with all Python versions ``sunpy`` supports. (`#6171 <https://github.com/sunpy/sunpy/pull/6171>`__)
-- Add support for upcoming parfive 2.0 release. (`#6243 <https://github.com/sunpy/sunpy/pull/6243>`__)
-- The primary sample-data URL will be changing from ``https://github.com/sunpy/sample-data/raw/master/sunpy/v1/`` to ``https://github.com/sunpy/data/raw/main/sunpy/v1/``.
-  We expect GitHub to redirect from the old URL for sometime but will eventually expire it.
-  The ``data.sunpy.org`` mirror will continue to be available. (`#6289 <https://github.com/sunpy/sunpy/pull/6289>`__)
-- Add support for downloading sample data from more than two mirror locations. (`#6295 <https://github.com/sunpy/sunpy/pull/6295>`__)
-- Timeseries data sources can now set the ``_peek_title`` class attribute
-  to set the default plot title produced when ``.peek()`` is called and the user
-  does not provide a custom title. (`#6304 <https://github.com/sunpy/sunpy/pull/6304>`__)
-- All internal code for limb drawing now uses :func:`~sunpy.visualization.drawing.limb`. (`#6332 <https://github.com/sunpy/sunpy/pull/6332>`__)
-- Add maintainer documentation on the backport bot (`#6355 <https://github.com/sunpy/sunpy/pull/6355>`__)
-- Switched to using the standard matrix-multiplication operator (available in Python 3.5+) instead of a custom function. (`#6376 <https://github.com/sunpy/sunpy/pull/6376>`__)
-- Fixed a colormap deprecation warning when importing the sunpy colormaps
-  with Matplotlib 3.6. (`#6379 <https://github.com/sunpy/sunpy/pull/6379>`__)
-- Removed custom tick label rotation from Lyra, EVE, and Norh timeseries sources, and grid drawing from NOAA and RHESSI sources. (`#6385 <https://github.com/sunpy/sunpy/pull/6385>`__)
-- Added tests and test data for `~sunpy.map.sources.SXTMap` (`#6436 <https://github.com/sunpy/sunpy/pull/6436>`__)
-- Fixed a bug where the private attribute ``_default_observer_coordinate`` for `~sunpy.map.GenericMap` was being used even when there was sufficient observer metadata in the header. (`#6447 <https://github.com/sunpy/sunpy/pull/6447>`__)
-- Tidy the GOES XRSTimesSeries tests and add two new XRS files to test. (`#6460 <https://github.com/sunpy/sunpy/pull/6460>`__)
-- Added a pre-commit hook for `codespell
-  <https://github.com/codespell-project/codespell>`__, and applied
-  spelling fixes throughout the package. (`#6574 <https://github.com/sunpy/sunpy/pull/6574>`__)
-
-
 v4.0.0 (2022-05-06)
 ===================
 
 Breaking Changes
 ----------------
 
 - When rotating images using the SciPy rotation method, the default behavior is now to clip the output range to the input range, which matches the default behavior of the scikit-image rotation method. (`#5867 <https://github.com/sunpy/sunpy/pull/5867>`__)
@@ -379,15 +67,15 @@
 - `sunpy.image.transform.affine_transform` and :meth:`sunpy.map.GenericMap.rotate`
   have both had their ``use_scipy`` arguments deprecated. Instead use the new
   ``method`` argument to select from the available rotation methods. (`#5916 <https://github.com/sunpy/sunpy/pull/5916>`__)
 - Added a Maxwell unit and any places where a conversion to Gauss occurs has been removed. (`#5998 <https://github.com/sunpy/sunpy/pull/5998>`__)
 - Add a basic HTML representation for `~sunpy.timeseries.TimeSeries`. (`#6032 <https://github.com/sunpy/sunpy/pull/6032>`__)
 - The minimum supported asdf version has been increased to 2.8.0 to allow future
   compatibility with the breaking changes planned for asdf 3.0.
-  In addition to this the `asdf-astropy <https://github.com/astropy/asdf-astropy>`__
+  In addtion to this the `asdf-astropy <https://github.com/astropy/asdf-astropy>`__
   package is now required to serialise and deserialise the sunpy coordinate frame
   classes to ASDF. (`#6057 <https://github.com/sunpy/sunpy/pull/6057>`__)
 - Added the option to rotate using `OpenCV <https://opencv.org>`__ when using :func:`sunpy.image.transform.affine_transform` or :meth:`sunpy.map.GenericMap.rotate` by specifying ``method='cv2'``.
   The OpenCV Python package must be installed on the system. (`#6089 <https://github.com/sunpy/sunpy/pull/6089>`__)
 
 
 Bug Fixes
@@ -404,15 +92,15 @@
   a particular column, units of ``u.dimensionless_unscaled`` are applied to that
   column and a warning raised.
 
   If you think a given unit should not be dimensionless and support should be
   added for it in sunpy, please raise an issue at
   https://github.com/sunpy/sunpy/issues. (`#5692 <https://github.com/sunpy/sunpy/pull/5692>`__)
 - The default ``id_type`` in :func:`sunpy.coordinates.get_horizons_coord` is now
-  `None` to match the default ``id_type`` in astroquery 0.4.4, which will search
+  `None` to match the deafult ``id_type`` in astroquery 0.4.4, which will search
   major bodies first, and if no major bodies are found, then search small bodies.
   For older versions of astroquery the default ``id_type`` used by
   :func:`~sunpy.coordinates.get_horizons_coord` is still ``'majorbody'``. (`#5707 <https://github.com/sunpy/sunpy/pull/5707>`__)
 - In consultation with JSOC, we now limit all JSOC downloads to one connection.
   This will override all connection user settings passed to the downloader. (`#5714 <https://github.com/sunpy/sunpy/pull/5714>`__)
 - Updated the ``plot`` methods on some timeseries classes to correctly label and format the time axis. (`#5720 <https://github.com/sunpy/sunpy/pull/5720>`__)
 - Fixed a long-standing bug where our logger could intercept Astropy warnings in addition to SunPy warnings, and thus could conflict with Astropy's logger. (`#5722 <https://github.com/sunpy/sunpy/pull/5722>`__)
@@ -444,15 +132,15 @@
 - Fixed plotting and peeking NORH timeseries data with ``pandas`` 1.4.0. (`#5830 <https://github.com/sunpy/sunpy/pull/5830>`__)
 - In the case where `sunpy.database.Database.fetch()` successfully downloads only some of the search results, a `~sunpy.database.PartialFetchError` is raised. This fixes a bug where the successful downloads would have been added to the database, but sometimes with incorrect metadata. (`#5835 <https://github.com/sunpy/sunpy/pull/5835>`__)
 - When getting IRIS files from the VSO, Fido was incorrectly labelling them as XML files. (`#5868 <https://github.com/sunpy/sunpy/pull/5868>`__)
 - `~sunpy.map.sources.HMIMap` now looks for ``'INSTRUME'`` instead of ``'TELESCOP'`` in order to support Helioviewer JPEG2000 versions of HMI data which do not preserve the ``'TELESCOP'`` keyword as expected in the JSOC standard. (`#5886 <https://github.com/sunpy/sunpy/pull/5886>`__)
 - Fixes a bug where the ``cmap`` and ``norm`` keyword arguments were ignored when calling
   `~sunpy.map.MapSequence.plot`. (`#5889 <https://github.com/sunpy/sunpy/pull/5889>`__)
 - Fix parsing of the GOES/XRS netcdf files to ignore leap seconds. (`#5915 <https://github.com/sunpy/sunpy/pull/5915>`__)
-- Fixed compatibility with ``h5netcdf>0.14`` when loading GOES netcdf files. (`#5920 <https://github.com/sunpy/sunpy/pull/5920>`__)
+- Fixed compatability with ``h5netcdf>0.14`` when loading GOES netcdf files. (`#5920 <https://github.com/sunpy/sunpy/pull/5920>`__)
 - Fixed bugs with the rebinning and per-keV calculation for Fermi/GBM summary lightcurves (`~sunpy.timeseries.sources.GBMSummaryTimeSeries`). (`#5943 <https://github.com/sunpy/sunpy/pull/5943>`__)
 - Fixed the unintentionally slow parsing of Fermi/GBM files (`~sunpy.timeseries.sources.GBMSummaryTimeSeries`). (`#5943 <https://github.com/sunpy/sunpy/pull/5943>`__)
 - Fixes a bug in `~sunpy.map.sources.SJIMap` where undefined variable was
   used when parsing the wavelength.
   Also fixes the unit parsing by removing the "corrected" string from the
   ``BUNIT`` keyword as "corrected DN" cannot be parsed as a valid FITS unit. (`#5968 <https://github.com/sunpy/sunpy/pull/5968>`__)
 - Fixed unit handling issue with `.GenericMap` and lowercasing the unit before it submits it to `astropy.units`. (`#5970 <https://github.com/sunpy/sunpy/pull/5970>`__)
@@ -488,22 +176,22 @@
 Internal Changes
 ----------------
 
 - Sped up the parsing of results from the VSO. For large queries this significantly
   reduces the time needed to perform a query to the VSO. (`#5681 <https://github.com/sunpy/sunpy/pull/5681>`__)
 - `sunpy.map.GenericMap.wcs` now checks that the scale property has the correct
   units whilst constructing the WCS. (`#5682 <https://github.com/sunpy/sunpy/pull/5682>`__)
-- Added `packaging <https://pypi.org/project/packaging/>`__ as a core dependency as distutils is now deprecated. (`#5713 <https://github.com/sunpy/sunpy/pull/5713>`__)
+- Added `packaging <https://pypi.org/project/packaging/>`__ as a core depedency as distutils is now deprecated. (`#5713 <https://github.com/sunpy/sunpy/pull/5713>`__)
 - `~sunpy.util.exceptions.SunpyWarning` is no longer a subclass of `~astropy.utils.exceptions.AstropyWarning`. (`#5722 <https://github.com/sunpy/sunpy/pull/5722>`__)
 - Running the tests now requires the ``pytest-xdist`` package. By
   default tests are *not* run in parallel, but can be configured to do so
   using ``pytest-xdist`` command line options. (`#5827 <https://github.com/sunpy/sunpy/pull/5827>`__)
 - Migrate the asdf infrastructure to the new style converters etc added in asdf
   2.8.0. This makes sure sunpy will be compatible with the upcoming asdf 3.0 release. (`#6057 <https://github.com/sunpy/sunpy/pull/6057>`__)
-- Declare in our dependencies that we are not compatible with asdf 3.0.0 until we
+- Declare in our dependancies that we are not compatible with asdf 3.0.0 until we
   are. (`#6077 <https://github.com/sunpy/sunpy/pull/6077>`__)
 - Improved performance of the code that parses dates in clients that use the
   `~sunpy.net.scraper.Scraper` to get available files. (`#6101 <https://github.com/sunpy/sunpy/pull/6101>`__)
 
 
 3.1.0 (2021-10-29)
 ==================
@@ -554,15 +242,15 @@
 Deprecations
 ------------
 
 - ``sunpy.util.scraper.Scraper`` has been moved into `sunpy.net`, please update your imports to be ``from sunpy.net import Scraper``. (`#5364 <https://github.com/sunpy/sunpy/pull/5364>`__)
 - Using "neighbour" as a resampling method in
   :func:`sunpy.image.resample.resample` is deprecated. Use "nearest" instead,
   which has the same effect. (`#5480 <https://github.com/sunpy/sunpy/pull/5480>`__)
-- The `sunpy.visualization.animator` subpackage has been spun out into the
+- The `sunpy.visualization.animator` subpackge has been spun out into the
   standalone `mpl-animators <https://pypi.org/project/mpl-animators>`_ package,
   with the exception of `~sunpy.visualization.animator.MapSequenceAnimator`.
   Please update your imports to replace ``sunpy.visualization.animator`` with
   ``mpl_animators``.
 
   This is primarily because the ``ndcube`` package now relies on the animator
   classes as well as `sunpy`. (`#5619 <https://github.com/sunpy/sunpy/pull/5619>`__)
@@ -670,18 +358,18 @@
   This fixes inconsistencies in the input and output world coordinate systems when a
   non-linear projection is used. (`#5295 <https://github.com/sunpy/sunpy/pull/5295>`__)
 - Inputs to the ``dimensions`` and ``offset`` arguments to
   :meth:`sunpy.map.GenericMap.superpixel` in units other than ``u.pix``
   (e.g. ```u.kpix``) are now handled correctly. (`#5301 <https://github.com/sunpy/sunpy/pull/5301>`__)
 - Fractional inputs to the ``dimensions`` and ``offset`` arguments to
   :meth:`sunpy.map.GenericMap.superpixel` were previously rounded using `int`
-  in the superpixel algorithm, but not assigned integer values in the new metadata.
-  This has now been changed so the rounding is correctly reflected in the metadata. (`#5301 <https://github.com/sunpy/sunpy/pull/5301>`__)
+  in the superpixel algorithm, but not assigned integer values in the new meatadata.
+  This has now been changed so the rounding is correctly reflected in the meatadata. (`#5301 <https://github.com/sunpy/sunpy/pull/5301>`__)
 - Remove runtime use of ``astropy.tests.helper.assert_quantity_allclose`` which
-  introduces a runtime dependency on ``pytest``. (`#5305 <https://github.com/sunpy/sunpy/pull/5305>`__)
+  introduces a runtime dependancy on ``pytest``. (`#5305 <https://github.com/sunpy/sunpy/pull/5305>`__)
 - :meth:`sunpy.map.GenericMap.resample` now keeps the reference coordinate of the
   WCS projection the same as the input map, and updates the reference pixel accordingly.
   This fixes inconsistencies in the input and output world coordinate systems when a
   non-linear projection is used. (`#5309 <https://github.com/sunpy/sunpy/pull/5309>`__)
 - Fix saving `.GenericMap` to an asdf file with version 2.8.0 of the asdf package. (`#5342 <https://github.com/sunpy/sunpy/pull/5342>`__)
 - When the limb is entirely visible, :meth:`sunpy.map.GenericMap.draw_limb` no
   longer plots an invisible patch for the hidden part of the limb and now returns
@@ -784,15 +472,15 @@
 
 3.0.0 (2021-05-14)
 ==================
 
 Backwards Incompatible Changes
 ------------------------------
 
-- ``sunpy.instr`` has been deprecated and will be removed in sunpy 3.1 in favour of `sunkit_instruments`.
+- ``sunpy.instr`` has been depreacted and will be removed in sunpy 3.1 in favour of `sunkit_instruments`.
   The code that is under ``sunpy.instr`` is imported via `sunkit_instruments` to ensure backwards comparability. (`#4526 <https://github.com/sunpy/sunpy/pull/4526>`__)
 - Several `sunpy.map.GenericMap` attributes have been updated to return `None` when the relevant piece of FITS metadata is missing. These are:
 
   - `~sunpy.map.GenericMap.exposure_time`, previously defaulted to zero seconds.
   - `~sunpy.map.GenericMap.measurement`, previously defaulted to zero.
   - `~sunpy.map.GenericMap.waveunit`, previously defaulted to ``u.one``.
   - `~sunpy.map.GenericMap.wavelength`, previously defaulted to zero. (`#5126 <https://github.com/sunpy/sunpy/pull/5126>`__)
@@ -918,18 +606,18 @@
   This fixes inconsistencies in the input and output world coordinate systems when a
   non-linear projection is used. (`#5295 <https://github.com/sunpy/sunpy/pull/5295>`__)
 - Inputs to the ``dimensions`` and ``offset`` arguments to
   :meth:`sunpy.map.GenericMap.superpixel` in units other than ``u.pix``
   (e.g. ```u.kpix``) are now handled correctly. (`#5301 <https://github.com/sunpy/sunpy/pull/5301>`__)
 - Fractional inputs to the ``dimensions`` and ``offset`` arguments to
   :meth:`sunpy.map.GenericMap.superpixel` were previously rounded using `int`
-  in the superpixel algorithm, but not assigned integer values in the new metadata.
-  This has now been changed so the rounding is correctly reflected in the metadata. (`#5301 <https://github.com/sunpy/sunpy/pull/5301>`__)
+  in the superpixel algorithm, but not assigned integer values in the new meatadata.
+  This has now been changed so the rounding is correctly reflected in the meatadata. (`#5301 <https://github.com/sunpy/sunpy/pull/5301>`__)
 - Remove runtime use of ``astropy.tests.helper.assert_quantity_allclose`` which
-  introduces a runtime dependency on ``pytest``. (`#5305 <https://github.com/sunpy/sunpy/pull/5305>`__)
+  introduces a runtime dependancy on ``pytest``. (`#5305 <https://github.com/sunpy/sunpy/pull/5305>`__)
 - :meth:`sunpy.map.GenericMap.resample` now keeps the reference coordinate of the
   WCS projection the same as the input map, and updates the reference pixel accordingly.
   This fixes inconsistencies in the input and output world coordinate systems when a
   non-linear projection is used. (`#5309 <https://github.com/sunpy/sunpy/pull/5309>`__)
 - Fix saving `.GenericMap` to an asdf file with version 2.8.0 of the asdf package. (`#5342 <https://github.com/sunpy/sunpy/pull/5342>`__)
 
 
@@ -1047,15 +735,15 @@
   to ``Fido.fetch``.
 
   This, while a breaking change for anyone accessing these response objects
   directly, will hopefully make working with ``Fido`` search results much easier. (`#4798 <https://github.com/sunpy/sunpy/pull/4798>`__)
 - Results from the `~sunpy.net.dataretriever.NOAAIndicesClient` and the
   `~sunpy.net.dataretriever.NOAAPredictClient` no longer has ``Start Time`` or
   ``End Time`` in their results table as the results returned from the client are
-  not dependent upon the time parameter of a search. (`#4798 <https://github.com/sunpy/sunpy/pull/4798>`__)
+  not dependant upon the time parameter of a search. (`#4798 <https://github.com/sunpy/sunpy/pull/4798>`__)
 - The ``sunpy.net.vso.QueryResponse.search`` method has been removed as it has not
   worked since the 1.0 release of sunpy. (`#4798 <https://github.com/sunpy/sunpy/pull/4798>`__)
 - The ``sunpy.net.hek.hek.HEKColumn`` class has been removed, the ``HEKTable`` class
   now uses the standard `astropy.table.Column` class. (`#4798 <https://github.com/sunpy/sunpy/pull/4798>`__)
 - The keys used to format file paths in ``Fido.fetch`` have changed. They are now
   more standardised across all the clients, as they are all extracted from the
   names of the columns in the results table.
@@ -1110,15 +798,15 @@
   use ``sunpy.map.Map.data.size`` instead. (`#4338 <https://github.com/sunpy/sunpy/pull/4338>`__)
 - ``sunpy.net.helio.HECClient.time_query`` is deprecated, `~sunpy.net.helio.HECClient.search`
   is the replacement. (`#4358 <https://github.com/sunpy/sunpy/pull/4358>`__)
 - ``sunpy.net.jsoc.attrs.Keys`` is deprecated; all fields are returned by default and can be filtered post search. (`#4358 <https://github.com/sunpy/sunpy/pull/4358>`__)
 - ``sunpy.net.hek.attrs.Time`` is deprecated; `~sunpy.net.attrs.Time` should be used instead. (`#4358 <https://github.com/sunpy/sunpy/pull/4358>`__)
 - Support for :func:`sunpy.coordinates.wcs_utils.solar_wcs_frame_mapping` to
   use the ``.heliographic_observer`` and ``.rsun`` attributes on a
-  `~astropy.wcs.WCS` is deprecated. (`#4620 <https://github.com/sunpy/sunpy/pull/4620>`__)
+  `~astropy.wcs.WCS` is depreacted. (`#4620 <https://github.com/sunpy/sunpy/pull/4620>`__)
 - The ``origin`` argument to `sunpy.map.GenericMap.pixel_to_world` and
   `sunpy.map.GenericMap.world_to_pixel` is deprecated.
 
   - If passing ``0``, not using the ``origin`` argument will have the same effect.
   - If passing ``1``, manually subtract 1 pixel from the input to ``pixel_to_world``,
     or manually add 1 pixel to the output of ``world_to_pixel``, and do not use the
     ``origin`` argument. (`#4700 <https://github.com/sunpy/sunpy/pull/4700>`__)
@@ -1137,15 +825,15 @@
   this only affects users interacting with the ``VSOClient`` object directly. (`#4798 <https://github.com/sunpy/sunpy/pull/4798>`__)
 
 
 Features
 --------
 
 
-- For :meth:`sunpy.map.GenericMap.quicklook` and :meth:`sunpy.map.MapSequence.quicklook` (also used for the HTML representation shown in Jupyter notebooks), the histogram is now shaded corresponding to the colormap of the plotted image.
+- For :meth:`sunpy.map.GenericMap.quicklook` and :meth:`sunpy.map.MapSequence.quicklook` (also used for the HTML reprsentation shown in Jupyter notebooks), the histogram is now shaded corresponding to the colormap of the plotted image.
   Clicking on the histogram will toggle an alternate version of the histogram. (`#4931 <https://github.com/sunpy/sunpy/pull/4931>`__)
 - Add an ``SRS_TABLE`` file to the sample data, and use it in the magnetogram
   plotting example. (`#4993 <https://github.com/sunpy/sunpy/pull/4993>`__)
 - Added a `sunpy.map.GenericMap.contour()` method to find the contours on a map. (`#3909 <https://github.com/sunpy/sunpy/pull/3909>`__)
 - Added a context manager (:meth:`~sunpy.coordinates.frames.Helioprojective.assume_spherical_screen`)
   to interpret `~sunpy.coordinates.frames.Helioprojective` coordinates as being on
   the inside of a spherical screen instead of on the surface of the Sun. (`#4003 <https://github.com/sunpy/sunpy/pull/4003>`__)
@@ -1198,15 +886,15 @@
 - Extended :meth:`~sunpy.timeseries.GenericTimeSeries.concatenate` and
   :meth:`~sunpy.timeseries.TimeSeriesMetaData.concatenate` to allow iterables. (`#4499 <https://github.com/sunpy/sunpy/pull/4499>`__)
 - Enable `~sunpy.coordinates.metaframes.RotatedSunFrame` to work with non-SunPy frames (e.g., `~astropy.coordinates.HeliocentricMeanEcliptic`). (`#4577 <https://github.com/sunpy/sunpy/pull/4577>`__)
 - Add support for `pathlib.Path` objects to be passed to `sunpy.timeseries.TimeSeries`. (`#4589 <https://github.com/sunpy/sunpy/pull/4589>`__)
 - Add support for GOES XRS netcdf files to be read as a `sunpy.timeseries.sources.XRSTimeSeries`. (`#4592 <https://github.com/sunpy/sunpy/pull/4592>`__)
 - Add `~sunpy.net.jsoc.attrs.Cutout` attr for requesting cutouts
   from JSOC via `~sunpy.net.jsoc.JSOCClient` and ``Fido``. (`#4595 <https://github.com/sunpy/sunpy/pull/4595>`__)
-- sunpy now sets auxiliary parameters on `sunpy.map.GenericMap.wcs` using the
+- sunpy now sets auxillary parameters on `sunpy.map.GenericMap.wcs` using the
   `astropy.wcs.Wcsprm.aux` attribute. This stores observer information, along with
   the reference solar radius if present. (`#4620 <https://github.com/sunpy/sunpy/pull/4620>`__)
 - The `~sunpy.coordinates.frames.HeliographicCarrington` frame now accepts the specification of ``observer='self'`` to indicate that the coordinate itself is also the observer for the coordinate frame.
   This functionality greatly simplifies working with locations of observatories that are provided in Carrington coordinates. (`#4659 <https://github.com/sunpy/sunpy/pull/4659>`__)
 - Add two new colormaps (``rhessi`` and ``std_gamma_2``) that are used for plotting RHESSI maps. (`#4665 <https://github.com/sunpy/sunpy/pull/4665>`__)
 - If either 'CTYPE1' or 'CTYPE2' are not present in map metadata, sunpy now assumes
   they are 'HPLN-TAN' and 'HPLT-TAN' (previously it assumed 'HPLN-   ' and 'HPLT-   ').
@@ -1307,15 +995,15 @@
   you are using data where the x/y axes are latitude/longitude, and now returns
   correct values in methods and properties that call ``pixel_to_world``,
   such as ``bottom_left_coord``, ``top_right_coord``, ``center``. (`#4700 <https://github.com/sunpy/sunpy/pull/4700>`__)
 - Added a warning when a 2D `~sunpy.coordinates.frames.Helioprojective` coordinate is upgraded to a 3D coordinate and the number type is lower precision than the native Python float.
   This 2D->3D upgrade is performed internally when transforming a 2D `~sunpy.coordinates.frames.Helioprojective` coordinate to any other coordinate frame. (`#4724 <https://github.com/sunpy/sunpy/pull/4724>`__)
 - All columns from a :meth:`sunpy.net.vso.vso.VSOClient.search` will now be shown. (`#4788 <https://github.com/sunpy/sunpy/pull/4788>`__)
 - The search results object returned from ``Fido.search``
-  (`~sunpy.net.fido_factory.UnifiedResponse`) now correctly counts all results in
+  (`~sunpy.net.fido_factory.UnifiedResponse`) now correcly counts all results in
   it's `~sunpy.net.fido_factory.UnifiedResponse.file_num` property. Note that
   because some ``Fido`` clients now return metadata only results, this is really
   the number of records and does not always correspond to the number of files
   that would be downloaded. (`#4798 <https://github.com/sunpy/sunpy/pull/4798>`__)
 - Improved the file processing logic for EVE L0CS files, which may have fixed a
   bug where the first line of data was parsed incorrectly. (`#4805 <https://github.com/sunpy/sunpy/pull/4805>`__)
 - Fixing the ``CROTA`` meta keyword in EUVI FITS to ``CROTAn`` standard. (`#4846 <https://github.com/sunpy/sunpy/pull/4846>`__)
@@ -1531,15 +1219,15 @@
   axes limits for the x axis were not correctly set. (`#4001 <https://github.com/sunpy/sunpy/pull/4001>`__)
 - Fixed passing in a list of URLs into `sunpy.map.GenericMap`, before it caused an error due to the wrong type being returned. (`#4007 <https://github.com/sunpy/sunpy/pull/4007>`__)
 - Fixed a bug with :func:`~sunpy.coordinates.transformations.transform_with_sun_center` where the global variable was sometimes restored incorrectly.
   This bug was most likely encountered if there was a nested use of this context manager. (`#4015 <https://github.com/sunpy/sunpy/pull/4015>`__)
 - Fixes a bug in fido_factory to allow  path="./" in fido.fetch(). (`#4058 <https://github.com/sunpy/sunpy/pull/4058>`__)
 - Prevented ``sunpy.io.fits.header_to_fits`` modifying the passed header in-place. (`#4067 <https://github.com/sunpy/sunpy/pull/4067>`__)
 - Strip out any unknown unicode from the HEK response to prevent it failing to load some results. (`#4088 <https://github.com/sunpy/sunpy/pull/4088>`__)
-- Fixed a bug in :func:`~sunpy.coordinates.ephemeris.get_body_heliographic_stonyhurst` that resulted in a error when requesting an array of locations in conjunction with enabling the light-travel-time correction. (`#4112 <https://github.com/sunpy/sunpy/pull/4112>`__)
+- Fixed a bug in :func:`~sunpy.coordinates.ephemeris.get_body_heliographic_stonyhurst` that resulted in a error when requesting an array of locations in conjuction with enabling the light-travel-time correction. (`#4112 <https://github.com/sunpy/sunpy/pull/4112>`__)
 - `sunpy.map.GenericMap.top_right_coord` and `~sunpy.map.GenericMap.center`
   have had their definitions clarified, and both have had off-by-one indexing
   errors fixed. (`#4121 <https://github.com/sunpy/sunpy/pull/4121>`__)
 - Fixed `sunpy.map.GenericMap.submap()` when scaled pixel units (e.g. ``u.mpix``)
   are used. (`#4127 <https://github.com/sunpy/sunpy/pull/4127>`__)
 - Fixed bugs in ``sunpy.util.scraper.Scraper.filelist``
   that resulted in error when the HTML page of URL opened by the scraper contains some "a" tags without "href" attribute
@@ -1589,15 +1277,15 @@
 - Improved the doc layout of `sunpy.data.sample`. (`#4034 <https://github.com/sunpy/sunpy/pull/4034>`__)
 - Made improvements to STEREO starfield gallery example. (`#4039 <https://github.com/sunpy/sunpy/pull/4039>`__)
 - Improved the documentation of `sunpy.map.GenericMap.resample`. (`#4043 <https://github.com/sunpy/sunpy/pull/4043>`__)
 - Updated the STEREO starfield example to use all of the information in the star catalog. (`#4116 <https://github.com/sunpy/sunpy/pull/4116>`__)
 - Mini-galleries are now easier to create in the documentation thanks to a custom Sphinx directive (``minigallery``).
   The page :ref:`sunpy-coordinates-rotatedsunframe` has an example of a mini-gallery at the bottom. (`#4124 <https://github.com/sunpy/sunpy/pull/4124>`__)
 - Added `sunpy.visualization.colormaps.color_tables` to the docs. (`#4182 <https://github.com/sunpy/sunpy/pull/4182>`__)
-- Made minor improvements to the map histogramming example. (`#4205 <https://github.com/sunpy/sunpy/pull/4205>`__)
+- Made minor improvments to the map histogramming example. (`#4205 <https://github.com/sunpy/sunpy/pull/4205>`__)
 - Add a warning to `sunpy.io` docs to recommend not using it for FITS (`#4208 <https://github.com/sunpy/sunpy/pull/4208>`__)
 
 
 Trivial/Internal Changes
 ------------------------
 
 - Removed un-used and un-tested code paths in the private ``_remove_lytaf_events`` function
@@ -1672,15 +1360,15 @@
 --------
 
 - Add a new `sunpy.data.manager` and `sunpy.data.cache` for dealing with versioned remote data within functions.
   Please see the `Remote Data Manager <https://docs.sunpy.org/en/latest/dev_guide/remote_data.html>`__ guide. (`#3124 <https://github.com/sunpy/sunpy/pull/3124>`__)
 - Added the coordinate frames `~sunpy.coordinates.frames.HeliocentricEarthEcliptic` (HEE), `~sunpy.coordinates.frames.GeocentricSolarEcliptic` (GSE), `~sunpy.coordinates.frames.HeliocentricInertial` (HCI), and `~sunpy.coordinates.frames.GeocentricEarthEquatorial` (GEI). (`#3212 <https://github.com/sunpy/sunpy/pull/3212>`__)
 - Added SunPy Map support for GOES SUVI images. (`#3269 <https://github.com/sunpy/sunpy/pull/3269>`__)
 - - Support APE14 for ``ImageAnimatorWCS`` in SunPy's visualization module (`#3275 <https://github.com/sunpy/sunpy/pull/3275>`__)
-- Add ability to disable progressbars when downloading files using `sunpy.net.helioviewer` and edited docstrings to mention this feature. (`#3280 <https://github.com/sunpy/sunpy/pull/3280>`__)
+- Add ability to disable progressbars when dowloading files using `sunpy.net.helioviewer` and edited docstrings to mention this feature. (`#3280 <https://github.com/sunpy/sunpy/pull/3280>`__)
 - Adds support for searching and downloading SUVI data. (`#3301 <https://github.com/sunpy/sunpy/pull/3301>`__)
 - Log all VSO XML requests and responses to the SunPy logger at the ``DEBUG``
   level. (`#3330 <https://github.com/sunpy/sunpy/pull/3330>`__)
 - Transformations between frames in `sunpy.coordinates` can now provide detailed debugging output.  Set the `logging` level to ``DEBUG`` to enable this output. (`#3339 <https://github.com/sunpy/sunpy/pull/3339>`__)
 - Added the `sunpy.coordinates.sun.carrington_rotation_time` function to
   compute the time of a given Carrington rotation number. (`#3360 <https://github.com/sunpy/sunpy/pull/3360>`__)
 - A new method has been added to remove columns from a
@@ -1723,15 +1411,15 @@
 
 - Fixed accuracy issues with the calculations of Carrington longitude (`~sunpy.coordinates.sun.L0`) and Carrington rotation number (`~sunpy.coordinates.sun.carrington_rotation_number`). (`#3178 <https://github.com/sunpy/sunpy/pull/3178>`__)
 - Updated :func:`sunpy.map.header_helper.make_fitswcs_header` to be more strict on the inputs it accepts. (`#3183 <https://github.com/sunpy/sunpy/pull/3183>`__)
 - Fix the calculation of ``rsun_ref`` in :func:`~sunpy.map.header_helper.make_fitswcs_header` and and
   ensure that the default reference pixel is indexed from 1. (`#3184 <https://github.com/sunpy/sunpy/pull/3184>`__)
 - Fixed the missing transformation between two `~sunpy.coordinates.HeliographicCarrington` frames with different observation times. (`#3186 <https://github.com/sunpy/sunpy/pull/3186>`__)
 - `sunpy.map.sources.AIAMap` and `sunpy.map.sources.HMIMap` will no longer assume
-  the existence of certain header keys. (`#3217 <https://github.com/sunpy/sunpy/pull/3217>`__)
+  the existance of certain header keys. (`#3217 <https://github.com/sunpy/sunpy/pull/3217>`__)
 - :func:`sunpy.map.header_helper.make_fitswcs_header` now supports specifying the map projection
   rather than defaulting to ``TAN``. (`#3218 <https://github.com/sunpy/sunpy/pull/3218>`__)
 - Fix the behaviour of
   ``sunpy.coordinates.frames.Helioprojective.calculate_distance`` if the
   representation isn't Spherical. (`#3219 <https://github.com/sunpy/sunpy/pull/3219>`__)
 - Fixed a bug where the longitude of a coordinate would not wrap at the expected angle following a frame transformation. (`#3223 <https://github.com/sunpy/sunpy/pull/3223>`__)
 - Fixed a bug where passing a time or time interval to the differential rotation function threw an error because the new observer was not in HGS. (`#3225 <https://github.com/sunpy/sunpy/pull/3225>`__)
@@ -1763,15 +1451,15 @@
 - Updated the URL for Fermi spacecraft-pointing files to use an HTTPS connection to HEASARC. (`#3381 <https://github.com/sunpy/sunpy/pull/3381>`__)
 - Fixed a bug where permission denied errors when downloading files are very verbose by adding an error message in `~sunpy.net.fido_factory.UnifiedDownloaderFactory.fetch`. (`#3417 <https://github.com/sunpy/sunpy/pull/3417>`__)
 - Fixed a malformed call to `astropy.time.Time` in a test, which resulted in an incorrect time scale (UTC instead of TT). (`#3418 <https://github.com/sunpy/sunpy/pull/3418>`__)
 - Fix incorrect files being included in the tarball, and docs missing from the
   tarball (`#3423 <https://github.com/sunpy/sunpy/pull/3423>`__)
 - Fixed a bug where clipping behavior had been enabled by default in the plotting normalizers for ``Map`` objects.  Clipping needs to be disabled to make use of the over/under/masked colors in the colormap. (`#3427 <https://github.com/sunpy/sunpy/pull/3427>`__)
 - Fix a bug with observer based frames that prevented a coordinate with an array of obstimes being transformed to other frames. (`#3455 <https://github.com/sunpy/sunpy/pull/3455>`__)
-- `sunpy.map.GenericMap` will no longer raise a warning if the position of the
+- `sunpy.map.GenericMap` will no longer raise a warning if the posisition of the
   observer is not known for frames that don't need an observer, i.e. heliographic
   frames. (`#3462 <https://github.com/sunpy/sunpy/pull/3462>`__)
 - Apply `os.path.expanduser` to `sunpy.map.map_factory.MapFactory` input
   before passing to `glob.glob` (`#3477 <https://github.com/sunpy/sunpy/pull/3477>`__)
 - Fix multiple instances of `sunpy.map` sources assuming the type of FITS Header
   values. (`#3497 <https://github.com/sunpy/sunpy/pull/3497>`__)
 - Fixed a bug with `~sunpy.coordinates.NorthOffsetFrame` where non-spherical representations for the north pole produced an error. (`#3517 <https://github.com/sunpy/sunpy/pull/3517>`__)
@@ -1843,15 +1531,15 @@
 - Removed ``sunpy.net.jsoc.attrs.Time`` because it served the same purpose as `sunpy.net.attrs.Time` after the switch to `astropy.time.Time`. (`#2694 <https://github.com/sunpy/sunpy/pull/2694>`__)
 - Remove unused ``**kwargs`` within TimeSeries functions. (`#2717 <https://github.com/sunpy/sunpy/pull/2717>`__)
 - Rotation matrices inside map objects were previously stored as numpy matrices, but are now
   stored as numpy arrays, as numpy will eventually remove their matrix datatype. See
   https://docs.scipy.org/doc/numpy/user/numpy-for-matlab-users.html for more information. (`#2719 <https://github.com/sunpy/sunpy/pull/2719>`__)
 - The ``sunpy.cm.show_colormaps`` function now accepts the keyword 'search' instead of 'filter'. (`#2731 <https://github.com/sunpy/sunpy/pull/2731>`__)
 - The keyword arguments to all client ``.fetch`` methods have been changed to
-  support the new parfive downloader and to ensure consistency across all Fido
+  support the new parfive downloader and to ensure consisteny across all Fido
   clients. (`#2797 <https://github.com/sunpy/sunpy/pull/2797>`__)
 - The Helioviewer client has been switched to using the newer Helioviewer API.
   This has meant that we have changed some of the keywords that were passed into client's methods.
   We have enforced that several keywords (observatory,instrument,detector,measurement) need to be defined otherwise the functions cannot return any data. (`#2801 <https://github.com/sunpy/sunpy/pull/2801>`__)
 - Maps no longer assume that the pixel units are arcseconds if the units aren't
   explicitly set. In addition to this if critical metadata is missing from when
   creating a map, the map will fail to initialize and will raise an error. (`#2847 <https://github.com/sunpy/sunpy/pull/2847>`__)
@@ -1965,16 +1653,16 @@
   does not exist. It will now create the directory when required. (`#2642 <https://github.com/sunpy/sunpy/pull/2642>`__)
 - Fix transformations into/out of Heliographic Stonyhurst frame when
   the coordinate representation is Cartesian. (`#2646 <https://github.com/sunpy/sunpy/pull/2646>`__)
 - Running the figure tests with ``setup.py test`` now saves the figures and the hashes to the same directory as setup.py. (`#2658 <https://github.com/sunpy/sunpy/pull/2658>`__)
 - ``sunpy.instr.fermi.met_to_utc`` now returns the correct utc time which takes into account the leap seconds that have passed. (`#2679 <https://github.com/sunpy/sunpy/pull/2679>`__)
 - Support passing Python file objects to ``sunpy.io.fits.write``. (`#2688 <https://github.com/sunpy/sunpy/pull/2688>`__)
 - Added DRMS to setup.py so sunpy[all] installs it as a dependency. (`#2693 <https://github.com/sunpy/sunpy/pull/2693>`__)
-- Fix eve 0cs timeseries separator regex to support Python 3.7 (`#2697 <https://github.com/sunpy/sunpy/pull/2697>`__)
-- Fix the bug which crashes `~sunpy.map.sources.LASCOMap` for when 'date-obs' is reformatted again from a self applied function. (`#2700 <https://github.com/sunpy/sunpy/pull/2700>`__)
+- Fix eve 0cs timeseries seperator regex to support Python 3.7 (`#2697 <https://github.com/sunpy/sunpy/pull/2697>`__)
+- Fix the bug which crashes `~sunpy.map.sources.LASCOMap` for when 'date-obs' is reformatted agian from a self applied function. (`#2700 <https://github.com/sunpy/sunpy/pull/2700>`__)
 - Change all instances of quantity_allclose to `astropy.units.allclose` this prevents pytest being needed to import `sunpy.coordinates` on Astropy 3 (`#2701 <https://github.com/sunpy/sunpy/pull/2701>`__)
 - Fix RHESSI obssum file downloading to include the final day in the time range. (`#2714 <https://github.com/sunpy/sunpy/pull/2714>`__)
 - Raise an error when transforming between HPC and HCC frames if the observer is not the same. (`#2725 <https://github.com/sunpy/sunpy/pull/2725>`__)
 - Replaces the existing LASCO C2 and C3 color maps with new ones that perform better with JP2 and Level 0.5, 1 data. (`#2731 <https://github.com/sunpy/sunpy/pull/2731>`__)
 - Do not attempt to save a FITS header comment for a keyword which is not in the header. This prevents an error on saving some maps after the metadata had been modified but not the comments. (`#2748 <https://github.com/sunpy/sunpy/pull/2748>`__)
 - Add support for `~sunpy.map.sources.HMIMap` objects as input to ``sunpy.instr.aia.aiaprep``. (`#2749 <https://github.com/sunpy/sunpy/pull/2749>`__)
 - User can convert between HPC and HCC coordinates with different observers. This is implemented by automatically transforming the coordinate into HGS and then changing observer, and then transforming back to HCC. (`#2754 <https://github.com/sunpy/sunpy/pull/2754>`__)
@@ -2020,15 +1708,15 @@
 - Minor changes to the developer guide regarding sprint labels. (`#2765 <https://github.com/sunpy/sunpy/pull/2765>`__)
 - Copyedited and corrected the solar cycles example. (`#2770 <https://github.com/sunpy/sunpy/pull/2770>`__)
 - Changed "online" mark to "remote_data" and made formatting of marks consistent. (`#2799 <https://github.com/sunpy/sunpy/pull/2799>`__)
 - Add a missing plot to the end of the units and coordinates guide. (`#2813 <https://github.com/sunpy/sunpy/pull/2813>`__)
 - Added gallery example showing how to access the SunPy colormaps (`#2865 <https://github.com/sunpy/sunpy/pull/2865>`__)
 - Added gallery example showing how to access the SunPy solar physics constants. (`#2882 <https://github.com/sunpy/sunpy/pull/2882>`__)
 - Major clean up of the developer documentation. (`#2951 <https://github.com/sunpy/sunpy/pull/2951>`__)
-- Overhaul of the install instructions for the guide section of our documentation. (`#3147 <https://github.com/sunpy/sunpy/pull/3147>`__)
+- Overhaul of the install intructions for the guide section of our documentation. (`#3147 <https://github.com/sunpy/sunpy/pull/3147>`__)
 
 
 Trivial/Internal Changes
 ------------------------
 
 - `~sunpy.time.parse_time` now uses `~functools.singledispatch` underneath. (`#2408 <https://github.com/sunpy/sunpy/pull/2408>`__)
 - Revert the handling of ``quantity_allclose`` now that `astropy/astropy#7252 <https://github.com/astropy/astropy/pull/7252>`__ is merged. This also bumps the minimum astropy version to 3.0.2. (`#2598 <https://github.com/sunpy/sunpy/pull/2598>`__)
@@ -2039,15 +1727,15 @@
 - Moved figure tests to Python 3.6. (`#2655 <https://github.com/sunpy/sunpy/pull/2655>`__)
 - Removed old metaclass used for Map and TimeSeries as we have now moved to Python 3.6. (`#2655 <https://github.com/sunpy/sunpy/pull/2655>`__)
 - Updated astropy_helpers to v3.0.2. (`#2655 <https://github.com/sunpy/sunpy/pull/2655>`__)
 - When running image tests, a comparison HTML page is now generated to show
   the generated images and expected images. (`#2660 <https://github.com/sunpy/sunpy/pull/2660>`__)
 - Change to using pytest-cov for coverage report generation to enable support for parallel builds (`#2667 <https://github.com/sunpy/sunpy/pull/2667>`__)
 - Use of `textwrap` to keep source code indented when multiline texts is used (`#2671 <https://github.com/sunpy/sunpy/pull/2671>`__)
-- Fix misspelling of private attribute ``_default_heliographic_latitude`` in map. (`#2730 <https://github.com/sunpy/sunpy/pull/2730>`__)
+- Fix mispelling of private attribute ``_default_heliographic_latitude`` in map. (`#2730 <https://github.com/sunpy/sunpy/pull/2730>`__)
 - Miscellaneous fixes to developer docs about building sunpy's documentation. (`#2825 <https://github.com/sunpy/sunpy/pull/2825>`__)
 - Changed ``sunpy.instr.aia.aiaprep`` to update BITPIX keyword to reflect the float64 dtype. (`#2831 <https://github.com/sunpy/sunpy/pull/2831>`__)
 - Remove warning from ``GenericMap.submap`` when using pixel ``Quantities`` as input. (`#2833 <https://github.com/sunpy/sunpy/pull/2833>`__)
 - Remove the usage of six and all ``__future__`` imports (`#2837 <https://github.com/sunpy/sunpy/pull/2837>`__)
 - Fix SunPy Coordinate tests with Astropy 3.1 (`#2838 <https://github.com/sunpy/sunpy/pull/2838>`__)
 - Stores entries from directories into database sorted by name. It adds mocks to the database user guide examples. (`#2873 <https://github.com/sunpy/sunpy/pull/2873>`__)
 - Fix all DeprecationWarning: invalid escape sequence. (`#2885 <https://github.com/sunpy/sunpy/pull/2885>`__)
@@ -2088,15 +1776,15 @@
 
 - Improve TimeSeriesBase docstring [#2399]
 - Validate that pytest-doctestplus is installed [#2388]
 - Fix use of self.wcs in plot in mapbase [#2398]
 - Updated docstring with pointer to access EVE data for other levels [#2402]
 - Fix broken links and redirections in documentation [#2403]
 - Fixes Documentation changes due to NumPy 1.14 [#2404]
-- Added docstrings to functions in download.py [#2415]
+- Added docstrings to functions in dowload.py [#2415]
 - Clean up database doc [#2414]
 - rhessi.py now uses sunpy.io instead of astropy.io [#2416]
 - Remove Gamma usage in Map [#2424]
 - Changed requirements to python-dateutil [#2426]
 - Clarify coordinate system definitions [#2429]
 - Improve Map Peek when using draw_grid [#2442]
 - Add HCC --> HGS test [#2443]
@@ -2331,15 +2019,15 @@
 =====
 
 -  Add Astropy 1.3 Support
 
 0.7.5
 =====
 
--  Fix test failure (mapbase) with 1.7.4
+-  Fix test faliure (mapbase) with 1.7.4
 -  Restrict supported Astropy version to 1.0<astropy<1.3
 -  Add Figure test env to SunPy repo.
 
 0.7.4
 =====
 
 -  Remove Map always forcing warnings on.
@@ -2631,15 +2319,15 @@
    matplotlib.animation.FuncAnimation object.
 
 0.5.1
 =====
 
 -  MAJOR FIX: map.rotate() now works correctly for all submaps and off
    center rotations.
--  HELIO URL updated, queries should now work as expected.
+-  HELIO URL updated, querys should now work as expected.
 -  All tabs removed from the code base.
 -  All tests now use tempfile rather than creating files in the current
    directory.
 -  Documentation builds under newer sphinx versions.
 -  ANA and JP2 tests are skipped if dependencies are missing.
 -  ANA tests are skipped on windows.
 
@@ -2666,16 +2354,16 @@
    (TRACE, RHESSI) were left out because SunPy is not able to read their
    FITS files.
 -  Added functions that implement image coalignment with support for
    MapCubes.
 -  Cleaned up the sunpy namespace, removed .units, /ssw and .sphinx.
    Also moved .coords .physics.transforms.
 -  Added contains functionality to TimeRange module
--  Added t-'now' to parse\_time to provide utcnow datetime.
--  Fixed time dependent functions (.sun) to default to t-'now'
+-  Added t-'now' to parse\_time to privide utcnow datetime.
+-  Fixed time dependant functions (.sun) to default to t-'now'
 -  Fixed solar\_semidiameter\_angular\_size
 -  Improved line quality and performances issues with map.draw\_grid()
 -  Remove deprecated make\_map command.
 
 0.4.2
 =====
 
@@ -2685,15 +2373,15 @@
 0.4.1
 =====
 
 -  Fix map.rotate() functionality
 -  Change of source for GOES data.
 -  Fix EIT test data and sunpy FITS saving
 -  Some documentation fixes
--  fix file paths to use os.path.join for platform independence.
+-  fix file paths to use os.path.join for platform independance.
 
 0.4.0
 =====
 
 -  **Major** documentation refactor. A far reaching re-write and
    restructure.
 -  Add a SunPy Database to store and search local data.
@@ -2707,28 +2395,28 @@
    https://docs.astropy.org/en/latest/constants/index.html
 -  Add some beta support for IRIS data products
 -  Add a new MapCubeAnimator class with interactive widgets which is
    returned by mapcube.peek().
 -  The Glymur library is now used to read JPEG2000 files.
 -  GOESLightCurve now supports all satellites.
 -  Add support for VSO queries through proxies.
--  Fix apparent Right Ascension calculations.
+-  Fix apparent Right Ascension calulations.
 -  LightCurve meta data member now an OrderedDict Instance
 
 0.3.2
 =====
 
 -  Pass draw\_limb arguments to patches.Circle
 -  Pass graw\_grid arguments to pyplot.plot()
 -  Fix README code example
 -  Fix Documentation links in potting guide
 -  Update to new EVE data URL
 -  Update LogicalLightcurve example in docs
 -  Improved InteractiveVSOClient documentation
--  GOESLightCurve now fails politely if no data is available.
+-  GOESLightCurve now fails politely if no data is avalible.
 
 Known Bugs:
 
 -  sunpy.util.unit\_conversion.to\_angstrom does not work if 'nm' is
    passed in.
 
 0.3.1
@@ -2742,46 +2430,46 @@
 0.3.0
 =====
 
 -  Removal of Optional PIL dependency
 -  Parse\_time now looks through nested lists/tuples
 -  Draw\_limb and draw\_grid are now implemented on MapCube and
    CompositeMap
--  Calculations for differential rotation added
+-  Caculations for differential roation added
 -  mapcube.plot() now runs a mpl animation with optional controls
 -  A basic Region of Interest framework now exists under sunpy.roi
 -  STEREO COR colour maps have been ported from solarsoft.
 -  sunpy.time.timerange has a split() method that divides up a time
    range into n equal parts.
 -  Added download progress bar
--  pyfits is deprecated in favor of Astropy
+-  pyfits is depricated in favor of Astropy
 
 spectra:
 
 -  Plotting has been refactorted to use a consistent interface
 -  spectra now no-longer inherits from numpy.ndarray instead has a .data
    attribute.
 
 Map: \* map now no-longer inherits from numpy.ndarray instead has a
 .data attribute. \* make\_map is deprecated in favor of Map which is a
 new factory class \* sunpy.map.Map is now sunpy.map.GenericMap \*
 mymap.header is now mymap.meta \* attributes of the map class are now
 read only, changes have to be made through map.meta \* new MapMeta class
 to replace MapHeader, MapMeta is not returned by sunpy.io \* The
-groundwork for GenericMap inheriting from astropy.NDData has been done,
+groundwork for GenericMap inherting from astropy.NDData has been done,
 there is now a NDDataStandin class to provide basic functionality.
 
 io: \* top level file\_tools improved to be more flexible and support
-multiple HDUs \* all functions in sunpy.io now assume multiple HDUs,
+multiple HDUs \* all functions in sunpy.io now assume mutliple HDUs,
 even JP2 ones. \* there is now a way to override the automatic filetype
 detection \* Automatic fits file detection improved \* extract\_waveunit
 added to io.fits for detection of common ways of storing wavelength unit
 in fits files.
 
--  A major re-work of all internal imports has resulted in a much cleaner
+-  A major re-work of all interal imports has resulted in a much cleaner
    namespace, i.e. sunpy.util.util is no longer used to import util.
 -  Some SOHO and STEREO files were not reading properly due to a
    date\_obs parameter.
 -  Sunpy will now read JP2 files without a comment parameter.
 -  Memory leak in Crotate patched
 -  Callisto: Max gap between files removed
```

### Comparing `sunpy-4.1.5/CITATION.rst` & `sunpy-4.1rc1/CITATION.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/LICENSE.rst` & `sunpy-4.1rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/PKG-INFO` & `sunpy-4.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy
-Version: 4.1.5
+Version: 4.1rc1
 Summary: SunPy core package: Python for Solar Physics
 Home-page: https://sunpy.org
 Download-URL: https://pypi.org/project/sunpy/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/sunpy/
@@ -50,15 +50,15 @@
 |Latest Version| |DOI| |matrix| |codecov| |Binder| |Powered by NumFOCUS|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/sunpy.svg
    :target: https://pypi.python.org/pypi/sunpy/
 .. |DOI| image:: https://zenodo.org/badge/2165383.svg
    :target: https://zenodo.org/badge/latestdoi/2165383
 .. |matrix| image:: https://img.shields.io/matrix/sunpy:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=openastronomy.modular.im
-   :target: https://app.element.io/#/room/#sunpy:openastronomy.org
+   :target: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
 .. |codecov| image:: https://codecov.io/gh/sunpy/sunpy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/sunpy/sunpy/main?filepath=examples
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
 
@@ -120,8 +120,8 @@
 This will walk you through getting set up for contributing.
 
 Code of Conduct
 ===============
 
 When you are interacting with the SunPy community you are asked to follow our `Code of Conduct <https://sunpy.org/coc>`__.
 
-.. _SunPy Chat: https://app.element.io/#/room/#sunpy:openastronomy.org
+.. _SunPy Chat: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
```

### Comparing `sunpy-4.1.5/README.rst` & `sunpy-4.1rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 |Latest Version| |DOI| |matrix| |codecov| |Binder| |Powered by NumFOCUS|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/sunpy.svg
    :target: https://pypi.python.org/pypi/sunpy/
 .. |DOI| image:: https://zenodo.org/badge/2165383.svg
    :target: https://zenodo.org/badge/latestdoi/2165383
 .. |matrix| image:: https://img.shields.io/matrix/sunpy:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=openastronomy.modular.im
-   :target: https://app.element.io/#/room/#sunpy:openastronomy.org
+   :target: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
 .. |codecov| image:: https://codecov.io/gh/sunpy/sunpy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/sunpy/sunpy/main?filepath=examples
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
 
@@ -75,8 +75,8 @@
 This will walk you through getting set up for contributing.
 
 Code of Conduct
 ===============
 
 When you are interacting with the SunPy community you are asked to follow our `Code of Conduct <https://sunpy.org/coc>`__.
 
-.. _SunPy Chat: https://app.element.io/#/room/#sunpy:openastronomy.org
+.. _SunPy Chat: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
```

### Comparing `sunpy-4.1.5/docs/Makefile` & `sunpy-4.1rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/coordinates/carrington.rst` & `sunpy-4.1rc1/docs/code_ref/coordinates/carrington.rst`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 Compared to |AA| and older methods of calculation
 -------------------------------------------------
 
 |AA| publishes the apparent sub-Earth Carrington longitude (|L0|), and these values include the stellar-aberration correction.
 Consequently, SunPy values will be consistently ~0.006 degrees (~20 arcseconds) greater than |AA| values, although these discrepancies are not always apparent at the printed precision (0.01 degrees).
 
-Since |AA| specifically tuned the IAU parameters to minimize the discrepancies with older methods of calculation under their prescription that includes the stellar-aberration correction, SunPy values will also be ~20 arcseconds greater than values calculated using older methods.
+Since |AA| specifically tuned the IAU parameters to minimize the discrepancies with older methods of calulation under their prescription that includes the stellar-aberration correction, SunPy values will also be ~20 arcseconds greater than values calculated using older methods.
 Be aware that older methods of calculation may not have accounted for the variable light travel time between the Sun and the Earth, which can cause additional discrepancies of up to ~5 arcseconds.
 
 |AA| does not appear to account for the difference in light travel time between the sub-Earth point on the Sun's surface and the center of the Sun (~2.3 lightseconds), which results in a fixed discrepancy of ~1.4 arcseconds in |L0|.
 However, this additional discrepancy is much smaller than the difference in treatment of stellar aberration.
 
 Compared to SPICE
 -----------------
```

### Comparing `sunpy-4.1.5/docs/code_ref/coordinates/index.rst` & `sunpy-4.1rc1/docs/code_ref/coordinates/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/coordinates/rotatedsunframe.rst` & `sunpy-4.1rc1/docs/code_ref/coordinates/rotatedsunframe.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/coordinates/velocities.rst` & `sunpy-4.1rc1/docs/code_ref/coordinates/velocities.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/coordinates/wcs.rst` & `sunpy-4.1rc1/docs/code_ref/coordinates/wcs.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/database.rst` & `sunpy-4.1rc1/docs/code_ref/database.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/io.rst` & `sunpy-4.1rc1/docs/code_ref/io.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/known_issues.rst` & `sunpy-4.1rc1/docs/code_ref/known_issues.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/map.rst` & `sunpy-4.1rc1/docs/code_ref/map.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/net.rst` & `sunpy-4.1rc1/docs/code_ref/net.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/stability.rst` & `sunpy-4.1rc1/docs/code_ref/stability.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/sunpy_stability.yaml` & `sunpy-4.1rc1/docs/code_ref/sunpy_stability.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/code_ref/timeseries.rst` & `sunpy-4.1rc1/docs/code_ref/timeseries.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/conf.py` & `sunpy-4.1rc1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # This needs to be done before sunpy is imported
 on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
 if on_rtd:
     os.environ['SUNPY_CONFIGDIR'] = '/home/docs/'
     os.environ['HOME'] = '/home/docs/'
     os.environ['LANG'] = 'C'
     os.environ['LC_ALL'] = 'C'
-    os.environ['PARFIVE_HIDE_PROGRESS'] = 'True'
+    os.environ['HIDE_PARFIVE_PROGESS'] = 'True'
 
 # -- Check for dependencies ----------------------------------------------------
 from sunpy.util import missing_dependencies_by_extra  # NOQA
 missing_requirements = missing_dependencies_by_extra("sunpy")["docs"]
 if missing_requirements:
     print(
         f"The {' '.join(missing_requirements.keys())} package(s) could not be found and "
```

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/backports.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/backports.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/ci_jobs.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/ci_jobs.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/code_standards.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/code_standards.rst`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 These can be private (see section above) or public.
 The decision is up to the developer, but if these might be useful for other packages within the sunpy ecosphere, they should be made public.
 
 Formatting
 ==========
 
-We enforce a minimum level of code style with our continuous integration (the name is ``sunpy.sunpy (python_codestyle [linux]``).
+We enforce a minimum level of code style with our continuous intergration (the name is ``sunpy.sunpy (python_codestyle [linux]``).
 This runs a tool called `pre-commit <https://pre-commit.com/>`__.
 
 The settings and tools we use for the pre-commit can be found in the file :file:`.pre-commit-config.yaml` at the root of the sunpy git repository.
 Some of the checks are:
 * Checks (but doesn't fix) various PEP8 issues with flake8.
 * Sort all imports in any Python files with isort.
 * Remove any unused variables or imports with autoflake.
```

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/conda_for_dependencies.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/conda_for_dependencies.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 Since the ``conda`` environment already has the complete set of dependencies for ``sunpy``, this call should install only ``sunpy`` and no additional packages.
 
 Editable Installation of ``sunpy``
 ==================================
 
 If you plan to modify the code of ``sunpy`` itself, you will want to perform an "editable install" of your local repository, via ``pip``, so that Python will link to your local repository.
-Normally it is discouraged to have an environment that mixes package installations via ``conda`` with package installations via ``pip`` because it can lead to environment states that confuse the ``conda`` solver.
+Normally it is discouraged to have an environment that mixes package installations via ``conda`` with package installations via ``pip`` because it can lead to enviroment states that confuse the ``conda`` solver.
 That is the reason why our instructions for new developers recommends that dependencies be installed exclusively via ``pip``.
 However, some of the dependencies in the complete set are difficult or even impossible to install via ``pip`` alone, yet are straightforward to install via ``conda``.
 
 Using the above ``conda`` environment, combined with a little care, it is possible to minimize that chance for any ``conda``/``pip`` conflicts.
 From the base directory of your local repository, install ``sunpy`` with some additional ``pip`` options:
 
 .. code:: bash
```

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/dependencies.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/dependencies.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/documentation.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/documentation.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/example_gallery.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/example_gallery.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/extending_fido.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/extending_fido.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ***************************************
 Extending Fido with New Sources of Data
 ***************************************
 
 Sunpy's data search and retrieval tool (``Fido``) is designed to be extensible, so that new sources of data or metadata can be supported, either inside or outside the sunpy core package.
 There are two ways of defining a new client, depending on the complexity of the web service.
 A "scraper" client inherits from `~sunpy.net.dataretriever.client.GenericClient` which provides helper methods for downloading from a list of URLs.
-If the service you want to add has easily accessible HTTP or FTP URLs that have a well defined folder and filename structure, this is probably the best approach.
+If the service you want to add has easily accesible HTTP or FTP URLs that have a well defined folder and filename structure, this is probably the best approach.
 If the service you want to add requires making requests to an API with parameters for the search and getting a list of results in return, then you probably want to write a "full" client.
 
 Before writing a new client, ensure you are familiar with how searches are specified by the `sunpy.net.attr` system, including combining them with logical operations.
 When choosing a name for your new client it should have the form ``<name>Client`` as sunpy will split the name the name of the class to extract the name of your client.
 The main place this is done is when constructing a `~.UnifiedResponse` object, where the name part can be used to index the response object.
 
 .. _new_scraper_client:
@@ -71,15 +71,15 @@
 * :meth:`~sunpy.net.dataretriever.client.GenericClient.pre_search_hook` which will convert the passed attrs to their representation in the URL.
 * :meth:`~sunpy.net.dataretriever.client.GenericClient.post_search_hook` which converts the retrieved metadata from a URL to the form in which they are desired to be represented in the response table.
 
 A good example of the use of these two methods is the `sunpy.net.dataretriever.sources.norh.NoRHClient` in sunpy.
 
 It may also be possible that the ``baseurl`` property needs to be customised based on attrs other than Time.
 Since `~sunpy.net.scraper.Scraper` doesn't currently support generating directories that have non-time variables, the :meth:`~sunpy.net.dataretriever.client.GenericClient.search` needs to be customised.
-The search method should in this case, generate a ``baseurl`` dependent on the values of these attrs, and then call ``super().search`` or `~sunpy.net.scraper.Scraper` for each ``baseurl`` generated.
+The search method should in this case, generate a ``baseurl`` dependant on the values of these attrs, and then call ``super().search`` or `~sunpy.net.scraper.Scraper` for each ``baseurl`` generated.
 For an example of a complex modification of the ``search()`` method see the implementation of `.SUVIClient.search`.
 
 Customizing the Downloader
 --------------------------
 
 There is no method for a client creator to override the `parfive.Downloader` that is used to fetch the files.
 This is because all downloads made by a single call to ``Fido.fetch`` share one instance of `parfive.Downloader`.
@@ -101,15 +101,15 @@
 --------
 
 Suppose any file of a data archive can be described by this URL ``https://some-domain.com/%Y/%m/%d/satname_{SatelliteNumber}_{Level}_%y%m%d%H%M%S_{any-2-digit-number}.fits``:
 
 ``baseurl`` becomes ``r'https://some-domain.com/%Y/%m/%d/satname_(\d){2}_(\d){1}_(\d){12}_(\d){2}\.fits'``.
 
 Note all variables in the filename are converted to regex that will match any possible value for it.
-A character enclosed within ``()`` followed by a number enclosed within ``{}`` is used to match the specified number of occurrences of that special sequence.
+A character enclosed within ``()`` followed by a number enclosed within ``{}`` is used to match the specified number of occurences of that special sequence.
 For example, ``%y%m%d%H%M%S`` is a twelve digit variable (with 2 digits for each item) and thus represented by ``r'(\d){12}'``.
 Note that ``\`` is used to escape the special character ``.``.
 
 ``pattern`` becomes ``'{}/{year:4d}/{month:2d}{day:2d}/satname_{SatelliteNumber:2d}_{Level:1d}_{:6d}{hour:2d}{minute:2d}{second:2d}_{:2d}.fits'``.
 Note the sole purpose of ``pattern`` is to extract the information from matched URL, using `~sunpy.extern.parse.parse`.
 So the desired key names for returned dictionary should be written in the ``pattern`` within ``{}``, and they should match with the ``attr.__name__``.
 
@@ -165,15 +165,15 @@
 .. code-block:: python
 
     (a.Time("2020/02/02", "2020/02/03") & a.Instrument("HMI")) | (a.Time("2020/02/02", "2020/02/03") & a.Instrument("AIA"))
 
 So you can process each element of the OR in turn without having to consult any other part of the query.
 
 If the query the user provided contains an OR statement you get passed an instance of `~sunpy.net.attr.AttrOr` and each sub-element of that `~sunpy.net.attr.AttrOr` will be `~sunpy.net.attr.AttrAnd` (or a single other attr class).
-If the user query doesn't contain an OR you get a single `~.Attr` instance or an `~.AttrAnd`.
+If the user query dosen't contain an OR you get a single `~.Attr` instance or an `~.AttrAnd`.
 
 For example you could get any of the following queries (using ``&`` for AND and ``|`` for OR):
 
 * ``(a.Instrument("AIA") & a.Time("2020/02/02", "2020/02/03")) | (a.Instrument("HMI") & a.Time("2020/02/02", "2020/02/03"))``
 * ``a.Time("2020/02/02", "2020/02/03")``
 * ``a.Instrument("AIA") & a.Time("2020/02/02", "2020/02/03")``
 * ``(a.Time(..) & a.Instrument("AIA") & a.Wavelength(30*u.nm, 31*u.nm)) | (a.Time(..) & a.Instrument("AIA") & a.Wavelength(30*u.nm, 31*u.nm))``
@@ -190,15 +190,15 @@
 This parsing and conversion of the query tree is deliberately not done using methods or attributes of the attrs themselves.
 The attrs should be independent of any client in their implementation, so they can be shared between the different ``Fido`` clients.
 
 A class is provided to facilitate this conversion, `~sunpy.net.attr.AttrWalker`.
 The `~sunpy.net.attr.AttrWalker` class consists of three main components:
 
 * **Creators**: The `~sunpy.net.attr.AttrWalker.create` method is one of two generic functions for which a different function is called for each Attr type.
-  The intended use for creators is to return a new object dependent on different attrs.
+  The intended use for creators is to return a new object dependant on different attrs.
   It is commonly used to dispatch on `~sunpy.net.attr.AttrAnd` and `~sunpy.net.attr.AttrOr`.
 
 * **Appliers**: The `~sunpy.net.attr.AttrWalker.apply` method is the same as `~sunpy.net.attr.AttrWalker.create` in that it is a generic function.
   The only difference between it and `~sunpy.net.attr.AttrWalker.create` is its intended use.
   Appliers are generally used to modify an object returned by a creator with the values or information contained in other Attrs.
 
 * **Converters**: Adding a converter to the walker adds the function to both the creator and the applier.
```

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/funding.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/funding.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/images/actions_check_pr.png` & `sunpy-4.1rc1/docs/dev_guide/contents/images/actions_check_pr.png`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/images/actions_summary_check.png` & `sunpy-4.1rc1/docs/dev_guide/contents/images/actions_summary_check.png`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/images/checks.png` & `sunpy-4.1rc1/docs/dev_guide/contents/images/checks.png`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/images/checks_pr.png` & `sunpy-4.1rc1/docs/dev_guide/contents/images/checks_pr.png`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/logger.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/logger.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/maintainer_workflow.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/maintainer_workflow.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/map_rotate_custom.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/map_rotate_custom.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/new_objects.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/new_objects.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/newcomers.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/newcomers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 If you have come across this page, you just might be new to the SunPy project - thanks for your interest in contributing to SunPy!
 SunPy is an open project that encourages anyone to contribute in any way possible.
 The people who help develop or contribute to SunPy are varied in ability and experience, with the vast majority being volunteers.
 
 If you have any questions, comments, or just want to say hello, we have an active `chat room`_ or a `mailing list`_.
 
-.. _chat room: https://app.element.io/#/room/#sunpy:openastronomy.org
+.. _chat room: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
 .. _mailing list: https://groups.google.com/forum/#!forum/sunpy
 
 How to Contribute to sunpy
 ==========================
 
 Not Code
 --------
@@ -66,15 +66,15 @@
 Generally the more people that can look over a pull request the better it will turn out and we encourage everyone to do so.
 
 .. _pull requests: https://github.com/sunpy/sunpy/pulls
 
 Code
 ----
 
-If you would prefer to code instead, the best way to start is to work on an existing and known `issues`_.
+If you would prefer to code instead, the best way to start is to work on an exisiting and known `issues`_.
 We have several repositories you can investigate.
 The main one is the sunpy repository with where all the known `issues`_ with sunpy are detailed.
 Each issue should have a series of labels that provide information about the nature of the issue.
 If you find an issue you'd like to work on, please make sure to add a comment to let people know that you are working on it! This will make it less likely that effort is duplicated.
 
 .. note::
 
@@ -142,15 +142,15 @@
 .. code:: bash
 
     $ conda config --add channels conda-forge
     $ conda create -n sunpy-dev pip
     $ conda activate sunpy-dev
 
 This will create a new conda environment called "sunpy-dev" and install the latest version of pip from the conda-forge channel.
-The next step is get a development version of sunpy.
+The next step is get a developement version of sunpy.
 This will require that `git`_ be installed.
 If you have a `GitHub`_ account, we suggest that you `fork`_ the `sunpy repository`_ (the fork button is to the top right) and **use that url for the clone step**.
 This will make submitting changes easier in the long term for you:
 
 .. warning::
 
     Do not clone the sunpy repository into ``$HOME/sunpy``. Depending on the operating system this location is used to store downloaded data files.
@@ -181,24 +181,24 @@
 .. _miniconda: https://conda.io/en/latest/miniconda.html
 .. _instructions are here: https://conda.io/projects/conda/en/latest/user-guide/install/index.html#installation
 .. _conda-forge: https://conda-forge.org/
 .. _git: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
 .. _GitHub: https://github.com/
 .. _fork: https://guides.github.com/activities/forking/
 .. _sunpy repository: https://github.com/sunpy/sunpy
-.. _ask here: https://app.element.io/#/room/#sunpy:openastronomy.org
+.. _ask here: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
 
 Checking the code you have written
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Now that you have written some code to address an issue.
 You will need to check two things:
 
 1. The changes you have made are correct, i.e., it fixes a bug or the feature works.
-   This requires you to run the code either manually or by writing/running a test function.
+   This requires you to run the code either manually or by writting/running a test function.
    `pytest`_ is the framework we use for this.
 
 2. The changes you have made follow the correct coding style.
    We follow the `PEP8`_ style for all Python code and depending on your setup, you can use a `linter program <https://realpython.com/python-code-quality/#how-to-improve-python-code-quality>`_ to check your code.
    For documentation, we follow the `numpydoc style <https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard>`_.
 
 We provide more more detail about our :ref:`test suite and how to write tests <testing>`, and how to :ref:`create and style documentation <docs_guidelines>`.
```

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/pr_checklist.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/pr_checklist.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/pr_review_procedure.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/pr_review_procedure.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/public_api.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/public_api.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/remote_data.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/remote_data.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/tests.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/tests.rst`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     >       assert func(3) == 5
     E       assert 4 == 5
     E        +  where 4 = func(3)
 
     test.py:5: AssertionError
     =========================== 1 failed in 0.07 seconds ===========================
 
-Sometimes the output from the test suite will have ``xfail`` meaning a test has passed although it has been marked as ``@pytest.mark.xfail``), or ``skipped`` meaning a test that has been skipped due to not meeting some condition (online and figure tests are the most common).
+Sometimes the output from the test suite will have ``xfail`` meaning a test has passed although it has been marked as ``@pytest.mark.xfail``), or ``skipped`` meaing a test that has been skipped due to not meeting some condition (online and figure tests are the most common).
 
 You need to use the option ``-rs`` for skipped tests and ``-rx`` for xfailed tests, respectively.
 Or use ``-rxs`` for detailed information on both skipped and xfailed tests.
 
 Where to put tests
 ------------------
```

### Comparing `sunpy-4.1.5/docs/dev_guide/contents/units_quantities.rst` & `sunpy-4.1rc1/docs/dev_guide/contents/units_quantities.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/dev_guide/index.rst` & `sunpy-4.1rc1/docs/dev_guide/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/diagrams/core_datatypes.dia` & `sunpy-4.1rc1/docs/diagrams/core_datatypes.dia`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/diagrams/map_class_hierarchy.dia` & `sunpy-4.1rc1/docs/diagrams/map_class_hierarchy.dia`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/diagrams/package_layout.dia` & `sunpy-4.1rc1/docs/diagrams/package_layout.dia`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/acquiring_data/database.rst` & `sunpy-4.1rc1/docs/guide/acquiring_data/database.rst`

 * *Files 0% similar despite different names*

```diff
@@ -534,15 +534,15 @@
      63    2011-05-08 00:00:03  2011-05-08 00:00:04        AIA    33.5    33.5
 
 5.3 Manually changing attributes
 ================================
 Attributes for entries in the database can be manually edited. The
 :meth:`Database.edit` method receives the database entry to be edited and any
 number of keyword arguments to describe which values to change and how. For
-example, to change the time entries that are ``None`` to the start of the
+example, to change the time entires that are ``None`` to the start of the
 observation time (because it's possible, not because it is accurate!):
 
     >>> for database_entry in database:
     ...     if database_entry.observation_time_end is None:
     ...         database.edit(database_entry, observation_time_end=database_entry.observation_time_start)
     ...
     >>> print(display_entries(
```

### Comparing `sunpy-4.1.5/docs/guide/acquiring_data/fido.rst` & `sunpy-4.1rc1/docs/guide/acquiring_data/fido.rst`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,22 @@
 ****************************
 
 This guide outlines how to search for and download data using the `~sunpy.net.Fido` interface for search and download.
 `~sunpy.net.Fido` is a unified interface for searching and fetching solar physics data irrespective of the underlying client or webservice through which the data is obtained.
 It therefore supplies a single, easy, and consistent way to obtain most forms of solar physics data.
 
 The `~sunpy.net.Fido` object is in `sunpy.net`.
-All the examples in this guide use ``Fido``, so lets start by importing it:
-
-.. code-block:: python
+All the examples in this guide use ``Fido``, so lets start by importing it::
 
     >>> from sunpy.net import Fido, attrs as a
 
 .. contents::
     :depth: 3
 
-Fido supports a number of different remote data sources. To see a list the Fido object can be printed:
-
-.. code-block:: python
+Fido supports a number of different remote data sources. To see a list the Fido object can be printed::
 
     >>> print(Fido)
     sunpy.net.Fido
     <BLANKLINE>
     Fido is a unified data search and retrieval tool.
     <BLANKLINE>
     It provides simultaneous access to a variety of online data sources, some
@@ -35,15 +31,15 @@
     <BLANKLINE>
     <BLANKLINE>
           Client                                                    Description
     ----------------- -------------------------------------------------------------------------------------------------------
     CDAWEBClient      Provides access to query and download from the Coordinated Data Analysis Web (CDAWeb).
     EVEClient         Provides access to Level 0CS Extreme ultraviolet Variability Experiment (EVE) data.
     GBMClient         Provides access to data from the Gamma-Ray Burst Monitor (GBM) instrument on board the Fermi satellite.
-    XRSClient         Provides access to several GOES XRS files archive.
+    XRSClient         Provides access to the GOES XRS fits files archive.
     SUVIClient        Provides access to data from the GOES Solar Ultraviolet Imager (SUVI).
     GONGClient        Provides access to the Magnetogram products of NSO-GONG synoptic Maps.
     LYRAClient        Provides access to the LYRA/Proba2 data archive.
     NOAAIndicesClient Provides access to the NOAA solar cycle indices.
     NOAAPredictClient Provides access to the NOAA SWPC predicted sunspot Number and 10.7 cm radio flux values.
     SRSClient         Provides access to the NOAA SWPC solar region summary data.
     NoRHClient        Provides access to the Nobeyama RadioHeliograph (NoRH) averaged correlation time series data.
@@ -62,26 +58,22 @@
 - `a.Time <sunpy.net.attrs.Time>`
 - `a.Instrument <sunpy.net.attrs.Instrument>`
 - `a.Wavelength <sunpy.net.attrs.Wavelength>`
 
 Some other attributes are client specific, and are found under client specific submodules, e.g. `attrs.vso <sunpy.net.vso.attrs>` and `attrs.jsoc <sunpy.net.jsoc.attrs>`.
 The full list of attributes can be found in the `attrs submodule reference <sunpy.net.attrs>`.
 
-Some search attributes need one or more values specifying, for example ``Time`` needs at least a start and an end date to specify a time range:
-
-.. code-block:: python
+Some search attributes need one or more values specifying, for example ``Time`` needs at least a start and an end date to specify a time range::
 
     >>> a.Time('2012/3/4', '2012/3/6')
     <sunpy.net.attrs.Time(2012-03-04 00:00:00.000, 2012-03-06 00:00:00.000)>
 
 For attributes that can take a range of different values, printing the attribute lists the values sunpy knows about.
 These values are updated with every release of sunpy, so may not be quite up to date!
-As an example:
-
-.. code-block:: python
+As an example::
 
     >>> print(a.Instrument)
     sunpy.net.attrs.Instrument
     <BLANKLINE>
     Specifies the Instrument name for the search.
     <BLANKLINE>
            Attribute Name          Client          Full Name                                           Description
@@ -96,26 +88,22 @@
     celias                      VSO         CELIAS                   Charge, Element, and Isotope Analysis System
     ...
 
 This is a full list of known values, a description, and which clients support those values (if you want to search using a specific data source).
 Printing attributes like this is supported for most attributes, including  client specific ones.
 These attributes also support tab-completion to auto to auto-fill the attribute name, for example typing ``a.jsoc.aia_f<TAB>`` in a jupyter notebook will show you the available attributes that start with "aia_f".
 
-To search for data use the ``Fido.search`` method:
-
-.. code-block:: python
+To search for data use the ``Fido.search`` method::
 
     >>> result = Fido.search(a.Time('2012/3/4', '2012/3/6'), a.Instrument.lyra, a.Level.two) # doctest: +REMOTE_DATA
 
 this returns an `~sunpy.net.fido_factory.UnifiedResponse` object containing all the search results that match the search attributes.
 This does not download the files; we'll learn how to do that later in :ref:`downloading_data`.
 
-To see a summary of the results print the result variable that came back from the previous search:
-
-.. code-block:: python
+To see a summary of the results print the result variable that came back from the previous search::
 
     >>> print(result)  # doctest: +REMOTE_DATA
     Results from 1 Provider:
     <BLANKLINE>
     3 Results from the LYRAClient:
     Source: http://proba2.oma.be/lyra/data/bsd
     <BLANKLINE>
@@ -124,17 +112,15 @@
     2012-03-04 00:00:00.000 2012-03-04 23:59:59.999       LYRA ...      ESA     2
     2012-03-05 00:00:00.000 2012-03-05 23:59:59.999       LYRA ...      ESA     2
     2012-03-06 00:00:00.000 2012-03-06 23:59:59.999       LYRA ...      ESA     2
     <BLANKLINE>
     <BLANKLINE>
 
 Queries can be made more flexible or specific by adding more attrs objects to the `~sunpy.net.Fido` search.
-As an example, specific passbands can be searched for by supplying an `~astropy.units.Quantity` to the `a.Wavelength <sunpy.net.attrs.Wavelength>` attribute:
-
-.. code-block:: python
+As an example, specific passbands can be searched for by supplying an `~astropy.units.Quantity` to the `a.Wavelength <sunpy.net.attrs.Wavelength>` attribute::
 
     >>> import astropy.units as u
     >>> Fido.search(a.Time('2012/3/4', '2012/3/6'), a.Instrument.norh,
     ...             a.Wavelength(17*u.GHz))  # doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
     Results from 1 Provider:
     <BLANKLINE>
@@ -146,17 +132,15 @@
     ----------------------- ----------------------- ... -------- ----------
     2012-03-04 00:00:00.000 2012-03-04 23:59:59.999 ...      NRO       17.0
     2012-03-05 00:00:00.000 2012-03-05 23:59:59.999 ...      NRO       17.0
     2012-03-06 00:00:00.000 2012-03-06 23:59:59.999 ...      NRO       17.0
     <BLANKLINE>
     <BLANKLINE>
 
-Data of a given cadence can also be specified using the `a.Sample <sunpy.net.attrs.Sample>` attribute:
-
-.. code-block:: python
+Data of a given cadence can also be specified using the `a.Sample <sunpy.net.attrs.Sample>` attribute::
 
     >>> Fido.search(a.Time('2012/3/4', '2012/3/6'), a.Instrument.aia,
     ...             a.Wavelength(171*u.angstrom), a.Sample(10*u.minute))  # doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
     Results from 1 Provider:
     <BLANKLINE>
     289 Results from the VSOClient:
@@ -188,17 +172,15 @@
     2012-03-05 23:50:00.000 ...
     2012-03-06 00:00:00.000 ...
     Length = 289 rows
     <BLANKLINE>
     <BLANKLINE>
 
 To search for data from multiple instruments, wavelengths, times etc., use the pipe ``|`` operator which joins queries using a logical ``OR`` operator.
-In this example we'll search for LYRA or RHESSI data in a given time range:
-
-.. code-block:: python
+In this example we'll search for LYRA or RHESSI data in a given time range::
 
     >>> Fido.search(a.Time('2012/3/4', '2012/3/4 02:00'),
     ...             a.Instrument.lyra | a.Instrument.rhessi)  # doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
     Results from 3 Providers:
     <BLANKLINE>
     2 Results from the LYRAClient:
@@ -215,34 +197,33 @@
            Start Time               End Time        Instrument ... Source Provider
     ----------------------- ----------------------- ---------- ... ------ --------
     2012-03-04 00:00:00.000 2012-03-04 23:59:59.999     RHESSI ... RHESSI     NASA
     <BLANKLINE>
     3 Results from the VSOClient:
     Source: http://vso.stanford.edu/cgi-bin/search
     <BLANKLINE>
-           Start Time               End Time        Source ... Extent Type   Size
-                                                           ...              Mibyte
-    ----------------------- ----------------------- ------ ... ----------- --------
-    2012-03-03 22:57:40.000 2012-03-04 00:33:20.000 RHESSI ... PARTIAL_SUN -0.00098
-    2012-03-04 00:33:20.000 2012-03-04 01:45:40.000 RHESSI ... PARTIAL_SUN -0.00098
-    2012-03-04 01:45:40.000 2012-03-04 02:09:00.000 RHESSI ... PARTIAL_SUN -0.00098
+           Start Time               End Time        ...   Size        Info
+                                                    ...  Mibyte
+    ----------------------- ----------------------- ... -------- --------------
+    2012-03-03 22:57:40.000 2012-03-04 00:33:20.000 ... -0.00098 RHESSI level-0
+    2012-03-04 00:33:20.000 2012-03-04 01:45:40.000 ... -0.00098 RHESSI level-0
+    2012-03-04 01:45:40.000 2012-03-04 02:09:00.000 ... -0.00098 RHESSI level-0
     <BLANKLINE>
     <BLANKLINE>
 
+
 Working with Search Results
 ***************************
 
 :meth:`Fido.search <sunpy.net.fido_factory.UnifiedDownloaderFactory.search>` can make multiple queries to multiple clients in one search.
 This means that the results of a call to search can contain many sets of records, called responses, from many clients.
 The results of a search are represented in a `~sunpy.net.fido_factory.UnifiedResponse` object, which provides access to all the response tables and allows some operations to be performed on all the results at once.
 `~sunpy.net.fido_factory.UnifiedResponse` acts both like a two dimensional array, where the first dimension is the response index and the second index is the row index, and a dictionary where you can index the responses by the name of the client.
 
-For example, the following code returns a response containing LYRA data from the `~sunpy.net.dataretriever.LYRAClient`, and EVE data from the `~sunpy.net.vso.VSOClient`:
-
-.. code-block:: python
+For example, the following code returns a response containing LYRA data from the `~sunpy.net.dataretriever.LYRAClient`, and EVE data from the `~sunpy.net.vso.VSOClient`::
 
     >>> from sunpy.net import Fido, attrs as a
     >>> results = Fido.search(a.Time("2012/1/1", "2012/1/2"), a.Level.two,
     ...                       a.Instrument.lyra | a.Instrument.eve)  # doctest: +REMOTE_DATA
     >>> results  # doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
     Results from 2 Providers:
@@ -254,56 +235,39 @@
     ----------------------- ----------------------- ---------- ... -------- -----
     2012-01-01 00:00:00.000 2012-01-01 23:59:59.999       LYRA ...      ESA     2
     2012-01-02 00:00:00.000 2012-01-02 23:59:59.999       LYRA ...      ESA     2
     <BLANKLINE>
     50 Results from the VSOClient:
     Source: http://vso.stanford.edu/cgi-bin/search
     <BLANKLINE>
-           Start Time               End Time        Source ... Extent Type   Size
-                                                           ...              Mibyte
-    ----------------------- ----------------------- ------ ... ----------- --------
-    2012-01-01 00:00:00.000 2012-01-01 01:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 00:00:00.000 2012-01-01 01:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 01:00:00.000 2012-01-01 02:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 01:00:00.000 2012-01-01 02:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 02:00:00.000 2012-01-01 03:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 02:00:00.000 2012-01-01 03:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 03:00:00.000 2012-01-01 04:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 03:00:00.000 2012-01-01 04:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 04:00:00.000 2012-01-01 05:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 04:00:00.000 2012-01-01 05:00:00.000    SDO ...    FULLDISK -0.00098
-                        ...                     ...    ... ...         ...      ...
-    2012-01-01 20:00:00.000 2012-01-01 21:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 20:00:00.000 2012-01-01 21:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 21:00:00.000 2012-01-01 22:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 21:00:00.000 2012-01-01 22:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 22:00:00.000 2012-01-01 23:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 22:00:00.000 2012-01-01 23:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 23:00:00.000 2012-01-02 00:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-01 23:00:00.000 2012-01-02 00:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-02 00:00:00.000 2012-01-02 01:00:00.000    SDO ...    FULLDISK -0.00098
-    2012-01-02 00:00:00.000 2012-01-02 01:00:00.000    SDO ...    FULLDISK -0.00098
+           Start Time               End Time        ...   Size         Info
+                                                    ...  Mibyte
+    ----------------------- ----------------------- ... -------- ----------------
+    2012-01-01 00:00:00.000 2012-01-01 01:00:00.000 ... -0.00098 L2Lines (merged)
+    2012-01-01 00:00:00.000 2012-01-01 01:00:00.000 ... -0.00098 L2Spectra (MEGS)
+    2012-01-01 01:00:00.000 2012-01-01 02:00:00.000 ... -0.00098 L2Lines (merged)
+                        ...                     ... ...      ...              ...
+    2012-01-01 23:00:00.000 2012-01-02 00:00:00.000 ... -0.00098 L2Spectra (MEGS)
+    2012-01-02 00:00:00.000 2012-01-02 01:00:00.000 ... -0.00098 L2Lines (merged)
+    2012-01-02 00:00:00.000 2012-01-02 01:00:00.000 ... -0.00098 L2Spectra (MEGS)
     Length = 50 rows
     <BLANKLINE>
     <BLANKLINE>
 
-If you then wanted to inspect just the LYRA data for the whole time range specified in the search, you would index this response to see just the results returned by the `~sunpy.net.dataretriever.LYRAClient`:
 
-.. code-block:: python
+If you then wanted to inspect just the LYRA data for the whole time range specified in the search, you would index this response to see just the results returned by the `~sunpy.net.dataretriever.LYRAClient`::
 
     >>> results[0, :]  # doctest: +REMOTE_DATA
     <sunpy.net.dataretriever.client.QueryResponse object at ...>
            Start Time               End Time        Instrument ... Provider Level
     ----------------------- ----------------------- ---------- ... -------- -----
     2012-01-01 00:00:00.000 2012-01-01 23:59:59.999       LYRA ...      ESA     2
     2012-01-02 00:00:00.000 2012-01-02 23:59:59.999       LYRA ...      ESA     2
 
-Or, equivalently:
-
-.. code-block:: python
+Or, equivalently::
 
     >>> results["lyra"]  # doctest: +REMOTE_DATA
     <sunpy.net.dataretriever.client.QueryResponse object at ...>
            Start Time               End Time        Instrument ... Provider Level
     ----------------------- ----------------------- ---------- ... -------- -----
     2012-01-01 00:00:00.000 2012-01-01 23:59:59.999       LYRA ...      ESA     2
     2012-01-02 00:00:00.000 2012-01-02 23:59:59.999       LYRA ...      ESA     2
@@ -313,82 +277,94 @@
 Note that the first (response) index is still necessary even if results are only found for a single client.
 So in this case the first result would be ``results[0, 0]`` rather than ``results[0]`` (the latter would return all results from the first - and only - client and is therefore the same as ``results``).
 
 As we have seen above the `~sunpy.net.fido_factory.UnifiedResponse` object contains many response tables which make up the search results.
 Each of the responses are `~sunpy.net.base_client.QueryResponseTable` objects, which are `astropy.table` objects meaning that you can interact with them and filter them like any other tabular data.
 This can be used to interact with results which are metadata only, i.e. searches from the HEK, or it can be used to reduce the number of files downloaded by `Fido.fetch <sunpy.net.fido_factory.UnifiedDownloaderFactory.fetch>`.
 
-For example if we did a query for some AIA and HMI data:
+For example if we did a query for some AIA and HMI data::
 
-.. code-block:: python
-
-    >>> results = Fido.search(a.Time("2020/01/01", "2020/01/01 00:01"), a.Instrument.aia | a.Instrument.hmi)  # doctest: +REMOTE_DATA
+    >>> results = Fido.search(a.Time("2020/01/01", "2020/01/01 00:05"), a.Instrument.aia | a.Instrument.hmi)  # doctest: +REMOTE_DATA
     >>> results  # doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
     Results from 2 Providers:
     <BLANKLINE>
-    41 Results from the VSOClient:
+    201 Results from the VSOClient:
     Source: http://vso.stanford.edu/cgi-bin/search
-    Total estimated size: 2.779 Gbyte
+    Total estimated size: 13.626 Gbyte
     <BLANKLINE>
-           Start Time               End Time        Source ... Extent Type   Size
-                                                           ...              Mibyte
-    ----------------------- ----------------------- ------ ... ----------- --------
-    2020-01-01 00:00:00.000 2020-01-01 00:00:01.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:04.000 2020-01-01 00:00:05.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:05.000 2020-01-01 00:00:06.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:05.000 2020-01-01 00:00:06.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:06.000 2020-01-01 00:00:07.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:09.000 2020-01-01 00:00:10.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:09.000 2020-01-01 00:00:10.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:11.000 2020-01-01 00:00:12.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:12.000 2020-01-01 00:00:13.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:14.000 2020-01-01 00:00:15.000    SDO ...    FULLDISK 64.64844
-                        ...                     ...    ... ...         ...      ...
-    2020-01-01 00:00:47.000 2020-01-01 00:00:48.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:48.000 2020-01-01 00:00:49.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:52.000 2020-01-01 00:00:53.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:52.000 2020-01-01 00:00:53.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:53.000 2020-01-01 00:00:54.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:54.000 2020-01-01 00:00:55.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:57.000 2020-01-01 00:00:58.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:57.000 2020-01-01 00:00:58.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:00:59.000 2020-01-01 00:01:00.000    SDO ...    FULLDISK 64.64844
-    2020-01-01 00:01:00.000 2020-01-01 00:01:01.000    SDO ...    FULLDISK 64.64844
-    Length = 41 rows
+           Start Time       ...
+                            ...
+    ----------------------- ...
+    2020-01-01 00:00:00.000 ...
+    2020-01-01 00:00:04.000 ...
+    2020-01-01 00:00:05.000 ...
+    2020-01-01 00:00:05.000 ...
+    2020-01-01 00:00:06.000 ...
+    2020-01-01 00:00:09.000 ...
+    2020-01-01 00:00:09.000 ...
+    2020-01-01 00:00:11.000 ...
+    2020-01-01 00:00:12.000 ...
+    2020-01-01 00:00:14.000 ...
+                        ... ...
+    2020-01-01 00:04:47.000 ...
+    2020-01-01 00:04:48.000 ...
+    2020-01-01 00:04:52.000 ...
+    2020-01-01 00:04:52.000 ...
+    2020-01-01 00:04:53.000 ...
+    2020-01-01 00:04:54.000 ...
+    2020-01-01 00:04:57.000 ...
+    2020-01-01 00:04:57.000 ...
+    2020-01-01 00:04:59.000 ...
+    2020-01-01 00:05:00.000 ...
+    Length = 201 rows
     <BLANKLINE>
-    3 Results from the VSOClient:
+    21 Results from the VSOClient:
     Source: http://vso.stanford.edu/cgi-bin/search
     <BLANKLINE>
-           Start Time               End Time        Source ... Extent Type   Size
-                                                           ...              Mibyte
-    ----------------------- ----------------------- ------ ... ----------- --------
-    2020-01-01 00:00:22.000 2020-01-01 00:00:23.000    SDO ...    FULLDISK -0.00098
-    2020-01-01 00:00:22.000 2020-01-01 00:00:23.000    SDO ...    FULLDISK -0.00098
-    2020-01-01 00:00:22.000 2020-01-01 00:00:23.000    SDO ...    FULLDISK -0.00098
+           Start Time               End Time        ...            Info
+                                                    ...
+    ----------------------- ----------------------- ... --------------------------
+    2020-01-01 00:00:22.000 2020-01-01 00:00:23.000 ... 45sec. Continuum intensity
+    2020-01-01 00:00:22.000 2020-01-01 00:00:23.000 ...         45sec. Magnetogram
+    2020-01-01 00:00:22.000 2020-01-01 00:00:23.000 ...         45sec. Dopplergram
+    2020-01-01 00:01:07.000 2020-01-01 00:01:08.000 ... 45sec. Continuum intensity
+    2020-01-01 00:01:07.000 2020-01-01 00:01:08.000 ...         45sec. Magnetogram
+    2020-01-01 00:01:07.000 2020-01-01 00:01:08.000 ...         45sec. Dopplergram
+    2020-01-01 00:01:52.000 2020-01-01 00:01:53.000 ... 45sec. Continuum intensity
+    2020-01-01 00:01:52.000 2020-01-01 00:01:53.000 ...         45sec. Magnetogram
+    2020-01-01 00:01:52.000 2020-01-01 00:01:53.000 ...         45sec. Dopplergram
+    2020-01-01 00:02:37.000 2020-01-01 00:02:38.000 ... 45sec. Continuum intensity
+    2020-01-01 00:02:37.000 2020-01-01 00:02:38.000 ...         45sec. Magnetogram
+    2020-01-01 00:02:37.000 2020-01-01 00:02:38.000 ...         45sec. Dopplergram
+    2020-01-01 00:03:22.000 2020-01-01 00:03:23.000 ... 45sec. Continuum intensity
+    2020-01-01 00:03:22.000 2020-01-01 00:03:23.000 ...         45sec. Magnetogram
+    2020-01-01 00:03:22.000 2020-01-01 00:03:23.000 ...         45sec. Dopplergram
+    2020-01-01 00:04:07.000 2020-01-01 00:04:08.000 ... 45sec. Continuum intensity
+    2020-01-01 00:04:07.000 2020-01-01 00:04:08.000 ...         45sec. Magnetogram
+    2020-01-01 00:04:07.000 2020-01-01 00:04:08.000 ...         45sec. Dopplergram
+    2020-01-01 00:04:52.000 2020-01-01 00:04:53.000 ... 45sec. Continuum intensity
+    2020-01-01 00:04:52.000 2020-01-01 00:04:53.000 ...         45sec. Magnetogram
+    2020-01-01 00:04:52.000 2020-01-01 00:04:53.000 ...         45sec. Dopplergram
     <BLANKLINE>
     <BLANKLINE>
 
 The VSO client returns a lot of information about the records, so the first thing we can do is show only the columns we are interested in.
-We can inspect all the available column names in all the responses with the `~.UnifiedResponse.all_colnames` property:
-
-.. code-block:: python
+We can inspect all the available column names in all the responses with the `~.UnifiedResponse.all_colnames` property::
 
     >>> results.all_colnames  # doctest: +REMOTE_DATA
-    ['End Time', 'Extent Length', 'Extent Type', 'Extent Width', 'Instrument', 'Physobs', 'Provider', 'Size', 'Source', 'Start Time', 'Wavelength', 'Wavetype', 'fileid']
-
-And then we can pick which ones to see with the :meth:`~.UnifiedResponse.show` method:
+    ['End Time', 'Extent Length', 'Extent Type', 'Extent Width', 'Info', 'Instrument', 'Physobs', 'Provider', 'Size', 'Source', 'Start Time', 'Wavelength', 'Wavetype', 'fileid']
 
-.. code-block:: python
+And then we can pick which ones to see with the :meth:`~.UnifiedResponse.show` method::
 
     >>> results.show("Start Time", "Instrument", "Physobs", "Wavelength")  # doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
     Results from 2 Providers:
     <BLANKLINE>
-    41 Results from the VSOClient:
+    201 Results from the VSOClient:
     Source: http://vso.stanford.edu/cgi-bin/search
     <BLANKLINE>
            Start Time       Instrument  Physobs     Wavelength
                                                      Angstrom
     ----------------------- ---------- --------- ----------------
     2020-01-01 00:00:00.000        AIA intensity   335.0 .. 335.0
     2020-01-01 00:00:04.000        AIA intensity   193.0 .. 193.0
@@ -397,127 +373,151 @@
     2020-01-01 00:00:06.000        AIA intensity   131.0 .. 131.0
     2020-01-01 00:00:09.000        AIA intensity   171.0 .. 171.0
     2020-01-01 00:00:09.000        AIA intensity   211.0 .. 211.0
     2020-01-01 00:00:11.000        AIA intensity     94.0 .. 94.0
     2020-01-01 00:00:12.000        AIA intensity   335.0 .. 335.0
     2020-01-01 00:00:14.000        AIA intensity 1600.0 .. 1600.0
                         ...        ...       ...              ...
-    2020-01-01 00:00:47.000        AIA intensity     94.0 .. 94.0
-    2020-01-01 00:00:48.000        AIA intensity   335.0 .. 335.0
-    2020-01-01 00:00:52.000        AIA intensity 1700.0 .. 1700.0
-    2020-01-01 00:00:52.000        AIA intensity   193.0 .. 193.0
-    2020-01-01 00:00:53.000        AIA intensity   304.0 .. 304.0
-    2020-01-01 00:00:54.000        AIA intensity   131.0 .. 131.0
-    2020-01-01 00:00:57.000        AIA intensity   171.0 .. 171.0
-    2020-01-01 00:00:57.000        AIA intensity   211.0 .. 211.0
-    2020-01-01 00:00:59.000        AIA intensity     94.0 .. 94.0
-    2020-01-01 00:01:00.000        AIA intensity   335.0 .. 335.0
-    Length = 41 rows
+    2020-01-01 00:04:47.000        AIA intensity     94.0 .. 94.0
+    2020-01-01 00:04:48.000        AIA intensity   335.0 .. 335.0
+    2020-01-01 00:04:52.000        AIA intensity 1700.0 .. 1700.0
+    2020-01-01 00:04:52.000        AIA intensity   193.0 .. 193.0
+    2020-01-01 00:04:53.000        AIA intensity   304.0 .. 304.0
+    2020-01-01 00:04:54.000        AIA intensity   131.0 .. 131.0
+    2020-01-01 00:04:57.000        AIA intensity   171.0 .. 171.0
+    2020-01-01 00:04:57.000        AIA intensity   211.0 .. 211.0
+    2020-01-01 00:04:59.000        AIA intensity     94.0 .. 94.0
+    2020-01-01 00:05:00.000        AIA intensity   335.0 .. 335.0
+    Length = 201 rows
     <BLANKLINE>
-    3 Results from the VSOClient:
+    21 Results from the VSOClient:
     Source: http://vso.stanford.edu/cgi-bin/search
     <BLANKLINE>
            Start Time       Instrument      Physobs          Wavelength
                                                               Angstrom
     ----------------------- ---------- ------------------ ----------------
     2020-01-01 00:00:22.000        HMI          intensity 6173.0 .. 6174.0
     2020-01-01 00:00:22.000        HMI LOS_magnetic_field 6173.0 .. 6174.0
     2020-01-01 00:00:22.000        HMI       LOS_velocity 6173.0 .. 6174.0
+    2020-01-01 00:01:07.000        HMI          intensity 6173.0 .. 6174.0
+    2020-01-01 00:01:07.000        HMI LOS_magnetic_field 6173.0 .. 6174.0
+    2020-01-01 00:01:07.000        HMI       LOS_velocity 6173.0 .. 6174.0
+    2020-01-01 00:01:52.000        HMI          intensity 6173.0 .. 6174.0
+    2020-01-01 00:01:52.000        HMI LOS_magnetic_field 6173.0 .. 6174.0
+    2020-01-01 00:01:52.000        HMI       LOS_velocity 6173.0 .. 6174.0
+    2020-01-01 00:02:37.000        HMI          intensity 6173.0 .. 6174.0
+    2020-01-01 00:02:37.000        HMI LOS_magnetic_field 6173.0 .. 6174.0
+    2020-01-01 00:02:37.000        HMI       LOS_velocity 6173.0 .. 6174.0
+    2020-01-01 00:03:22.000        HMI          intensity 6173.0 .. 6174.0
+    2020-01-01 00:03:22.000        HMI LOS_magnetic_field 6173.0 .. 6174.0
+    2020-01-01 00:03:22.000        HMI       LOS_velocity 6173.0 .. 6174.0
+    2020-01-01 00:04:07.000        HMI          intensity 6173.0 .. 6174.0
+    2020-01-01 00:04:07.000        HMI LOS_magnetic_field 6173.0 .. 6174.0
+    2020-01-01 00:04:07.000        HMI       LOS_velocity 6173.0 .. 6174.0
+    2020-01-01 00:04:52.000        HMI          intensity 6173.0 .. 6174.0
+    2020-01-01 00:04:52.000        HMI LOS_magnetic_field 6173.0 .. 6174.0
+    2020-01-01 00:04:52.000        HMI       LOS_velocity 6173.0 .. 6174.0
     <BLANKLINE>
     <BLANKLINE>
 
 To give an example of filtering post-search, let's only return the rows in the table which are line-of-sight magnetograms from HMI or the 94Å passband from AIA.
-You can also always do this filtering with the `a.Physobs <sunpy.net.attrs.Physobs>` and `a.Wavelength <sunpy.net.attrs.Wavelength>` attrs in the search command.
-
-First we split the results in to a table for AIA and a table for HMI:
+You can also always do this filtering with the `a.vso.Physobs <sunpy.net.attrs.Physobs>` and `a.Wavelength <sunpy.net.attrs.Wavelength>` attrs in the search command.
 
-.. code-block:: python
+First we split the results in to a table for AIA and a table for HMI::
 
    >>> aia, hmi = results  # doctest: +REMOTE_DATA
 
-We can use boolean indexing to match the value of the ``"Physobs"`` column:
-
-.. code-block:: python
+We can use boolean indexing to match the value of the ``"Physobs"`` column::
 
     >>> hmi_los = hmi[hmi["Physobs"] == "LOS_magnetic_field"]  # doctest: +REMOTE_DATA
     >>> hmi_los.show("Start Time", "Instrument", "Wavelength", "Physobs")  # doctest: +REMOTE_DATA
     <sunpy.net.vso.table_response.VSOQueryResponseTable object at ...>
            Start Time       Instrument    Wavelength         Physobs
                                            Angstrom
     ----------------------- ---------- ---------------- ------------------
     2020-01-01 00:00:22.000        HMI 6173.0 .. 6174.0 LOS_magnetic_field
+    2020-01-01 00:01:07.000        HMI 6173.0 .. 6174.0 LOS_magnetic_field
+    2020-01-01 00:01:52.000        HMI 6173.0 .. 6174.0 LOS_magnetic_field
+    2020-01-01 00:02:37.000        HMI 6173.0 .. 6174.0 LOS_magnetic_field
+    2020-01-01 00:03:22.000        HMI 6173.0 .. 6174.0 LOS_magnetic_field
+    2020-01-01 00:04:07.000        HMI 6173.0 .. 6174.0 LOS_magnetic_field
+    2020-01-01 00:04:52.000        HMI 6173.0 .. 6174.0 LOS_magnetic_field
 
-To match the ``"Wavelength"`` column we need to account for the fact that VSO results return a wavelength range of ``[min, max]`` so we match the min:
-
-.. code-block:: python
+To match the ``"Wavelength"`` column we need to account for the fact that VSO results return a wavelength range of ``[min, max]`` so we match the min::
 
     >>> aia_94 = aia[aia["Wavelength"][:, 0] == 94 * u.AA]  # doctest: +REMOTE_DATA
     >>> aia_94.show("Start Time", "Instrument", "Wavelength", "Physobs")  # doctest: +REMOTE_DATA
     <sunpy.net.vso.table_response.VSOQueryResponseTable object at ...>
            Start Time       Instrument  Wavelength   Physobs
                                          Angstrom
     ----------------------- ---------- ------------ ---------
     2020-01-01 00:00:11.000        AIA 94.0 .. 94.0 intensity
     2020-01-01 00:00:23.000        AIA 94.0 .. 94.0 intensity
     2020-01-01 00:00:35.000        AIA 94.0 .. 94.0 intensity
     2020-01-01 00:00:47.000        AIA 94.0 .. 94.0 intensity
     2020-01-01 00:00:59.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:01:11.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:01:23.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:01:35.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:01:47.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:01:59.000        AIA 94.0 .. 94.0 intensity
+                        ...        ...          ...       ...
+    2020-01-01 00:03:11.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:03:23.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:03:35.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:03:47.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:03:59.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:04:11.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:04:23.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:04:35.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:04:47.000        AIA 94.0 .. 94.0 intensity
+    2020-01-01 00:04:59.000        AIA 94.0 .. 94.0 intensity
+    Length = 25 rows
 
 .. warning::
 
-   While you can reduce the number of columns and rows in the results, the ``fetch()`` method that downloads data may need certain columns to be present to successfully download the files.
+   While you can reduce the number of columns and rows in the results, the ``fetch()`` method that downloades data may need certain columns to be present to successfully download the files.
    It is therefore highly recommended that if you are planning on downloading data you do not slice out columns, but instead use ``.show()`` to only display the ones you are interested in.
 
+
 .. _downloading_data:
 
 Downloading data
 ****************
 Once you have located your files via a `Fido.search <sunpy.net.fido_factory.UnifiedDownloaderFactory.search>`, you can download them via `Fido.fetch <sunpy.net.fido_factory.UnifiedDownloaderFactory.fetch>`.
-Here we'll just download the first file in the result:
-
-.. code-block:: python
+Here we'll just download the first file in the result::
 
     >>> downloaded_files = Fido.fetch(results[0, 0]) # doctest: +REMOTE_DATA
     >>> downloaded_files # doctest: +REMOTE_DATA
     <parfive.results.Results object at ...>
     ['.../aia_lev1_335a_2020_01_01t00_00_00_64z_image_lev1.fits']
 
 This downloads the files to the location set in the sunpy config file.
 It also returns a `parfive.Results` object ``downloaded_files``, which contains local file paths to all the downloaded data.
 
-You can also explicitly specify the path to which you want the data downloaded:
-
-.. code-block:: python
+You can also explicitly specify the path to which you want the data downloaded::
 
   >>> downloaded_files = Fido.fetch(results, path='/ThisIs/MyPath/to/Data/{file}')  # doctest: +SKIP
 
 This downloads the query results into the directory ``/ThisIs/MyPath/to/Data``, naming each downloaded file with the filename ``{file}`` obtained from the client.
 You can also use other properties of the returned query to define the path where the data is saved.
-For example, to save the data to a subdirectory named after the instrument, use:
-
-.. code-block:: python
+For example, to save the data to a subdirectory named after the instrument, use::
 
     >>> downloaded_files = Fido.fetch(results, path='./{instrument}/{file}')  # doctest: +SKIP
 
-You can see the list of options that can be specified in path for all the files to be downloaded with ``results.path_format_keys``:
-
-.. code-block:: python
+You can see the list of options that can be specified in path for all the files to be downloaded with ``results.path_format_keys``::
 
     >>> sorted(results.path_format_keys()) # doctest: +REMOTE_DATA
-    ['end_time', 'extent_length', 'extent_type', 'extent_width', 'fileid', 'instrument', 'physobs', 'provider', 'size', 'source', 'start_time', 'wavelength', 'wavetype']
+    ['end_time', 'extent_length', 'extent_type', 'extent_width', 'fileid', 'info', 'instrument', 'physobs', 'provider', 'size', 'source', 'start_time', 'wavelength', 'wavetype']
 
 Retrying Downloads
 ^^^^^^^^^^^^^^^^^^
 If any files failed to download, the progress bar will show an incomplete number of files (i.e. 100/150) and the `parfive.Results` object will contain a list of the URLs that failed to transfer and the error associated with them.
-This can be accessed with the ``.errors`` attribute or by printing the `~parfive.Results` object:
-
-.. code-block:: python
+This can be accessed with the ``.errors`` attribute or by printing the `~parfive.Results` object::
 
     >>> print(downloaded_files.errors)  # doctest: +SKIP
 
-The transfer can be retried by passing the `parfive.Results` object back to `Fido.fetch <sunpy.net.fido_factory.UnifiedDownloaderFactory.fetch>`:
-
-.. code-block:: python
+The transfer can be retried by passing the `parfive.Results` object back to `Fido.fetch <sunpy.net.fido_factory.UnifiedDownloaderFactory.fetch>`::
 
     >>> downloaded_files = Fido.fetch(downloaded_files)  # doctest: +SKIP
 
 doing this will append any newly downloaded file names to the list and replace the ``.errors`` list with any errors that occurred during the second attempt.
```

### Comparing `sunpy-4.1.5/docs/guide/acquiring_data/hek.rst` & `sunpy-4.1rc1/docs/guide/acquiring_data/hek.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/acquiring_data/helioviewer.rst` & `sunpy-4.1rc1/docs/guide/acquiring_data/helioviewer.rst`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ``HelioviewerClient().get_data_sources`` is replaced by :func:`hvpy.getDataSources`.
 
 .. code-block:: python
 
    >>> import hvpy
    >>> hvpy.getDataSources()  # doctest: +REMOTE_DATA
-   {...'SDO': {...'HMI': {'continuum': {'sourceId': 18,
+   {'SDO': {'HMI': {'continuum': {'sourceId': 18,
    ...
 
 ``HelioviewerClient().get_closest_image`` is replaced by :func:`hvpy.getClosestImage`.
 
 .. code-block:: python
 
    >>> from datetime import datetime
```

### Comparing `sunpy-4.1.5/docs/guide/acquiring_data/jsoc.rst` & `sunpy-4.1rc1/docs/guide/acquiring_data/jsoc.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/acquiring_data/sample-data.rst` & `sunpy-4.1rc1/docs/guide/acquiring_data/sample-data.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/coordinates.rst` & `sunpy-4.1rc1/docs/guide/coordinates.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/customization.rst` & `sunpy-4.1rc1/docs/guide/customization.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/data_types/maps.rst` & `sunpy-4.1rc1/docs/guide/data_types/maps.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/data_types/timeseries.rst` & `sunpy-4.1rc1/docs/guide/data_types/timeseries.rst`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 .. code-block:: python
 
     >>> my_ts_list = ts.TimeSeries('filepath1', 'filepath2', source='XRS')   # doctest: +SKIP
     >>> my_ts_list = ts.TimeSeries('/goesdirectory/', source='XRS')   # doctest: +SKIP
     >>> my_ts_list = ts.TimeSeries(glob, source='XRS')   # doctest: +SKIP
 
-When manually specifying the source this functionality will only work with files from the same single source, generating a source specific child of the `~sunpy.timeseries.GenericTimeSeries` class such as the `~sunpy.timeseries.sources.goes.XRSTimeSeries` above.
+When manually specifing the source this functionality will only work with files from the same single source, generating a source specific child of the `~sunpy.timeseries.GenericTimeSeries` class such as the `~sunpy.timeseries.sources.goes.XRSTimeSeries` above.
 
 Instead of creating a list of one TimeSeries object per file, you can create a single time series from multiple files using the keyword argument ``concatenate=True``:
 
 .. code-block:: python
 
     >>> my_ts = ts.TimeSeries(sunpy.data.sample.GOES_XRS_TIMESERIES, sunpy.data.sample.GOES_XRS_TIMESERIES, source='XRS', concatenate=True)  # doctest: +REMOTE_DATA
```

### Comparing `sunpy-4.1.5/docs/guide/index.rst` & `sunpy-4.1rc1/docs/guide/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/logger.rst` & `sunpy-4.1rc1/docs/guide/logger.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/plotting.rst` & `sunpy-4.1rc1/docs/guide/plotting.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/ssw.rst` & `sunpy-4.1rc1/docs/guide/ssw.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/time.rst` & `sunpy-4.1rc1/docs/guide/time.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/tour.rst` & `sunpy-4.1rc1/docs/guide/tour.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/troubleshooting.rst` & `sunpy-4.1rc1/docs/guide/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/guide/units.rst` & `sunpy-4.1rc1/docs/guide/units.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 *****
 
 This section of the guide talks about representing physical units in sunpy.
 sunpy makes use of the `astropy.units` for this task.
 
 Quantity objects
 ================
-All functions in sunpy that accept or return numbers associated with physical quantities accept and return `~astropy.units.Quantity` objects.
+All functions in sunpy that accept or return numbers associated with physcial quantities accept and return `~astropy.units.Quantity` objects.
 These objects represent a number (or an array of numbers) and a unit.
 This means sunpy is always explicit about the units associated with a value.
 Quantities and units are powerful tools for keeping track of variables with a physical meaning and make it straightforward to convert the same physical quantity into different units.
 
 To use units we must first import them from Astropy.
 To save on typing it's standard practice to import the units module as ``u``::
```

### Comparing `sunpy-4.1.5/docs/index.rst` & `sunpy-4.1rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/installation.rst` & `sunpy-4.1rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/make.bat` & `sunpy-4.1rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/nitpick-exceptions` & `sunpy-4.1rc1/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/0.8.rst` & `sunpy-4.1rc1/docs/whatsnew/0.8.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/0.9.rst` & `sunpy-4.1rc1/docs/whatsnew/0.9.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 * 807 commits have been added since 0.8
 * 310 issues have been closed since 0.8
 * 147 pull requests have been merged since 0.8
 * 34 people have contributed since 0.8
 * 19 new contributors
 
 There have been numerous improvements to large parts of SunPy, notably in the content of SunPy's documentation, and the continuous integration testing of SunPy.
-In addition, SunPy coordinate system functionality has been improved, and the transformation between SunPy specific coordinate systems and those implemented by Astropy is now tested.
+In addition, SunPy co-ordinate system functionality has been improved, and the transformation between SunPy specific co-ordinate systems and those implemented by Astropy is now tested.
 The `sunpy.map.CompositeMap` object has received numerous bugfixes, improving its functionality.
 Bugfixes for various animation functionality have also been implemented.
 
 .. _whatsnew-0.9-python:
 
 Supported versions of Python
 ============================
```

### Comparing `sunpy-4.1.5/docs/whatsnew/1.0.rst` & `sunpy-4.1rc1/docs/whatsnew/1.0.rst`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 All messages provided by SunPy use a new logging facility which is based on the Python logging module rather than print statements.
 
 Messages can have one of several levels, in increasing order of importance:
 
 * DEBUG: Detailed information, typically of interest only when diagnosing problems.
 * INFO: A message conveying information about the current task, and confirming that things are working as expected.
 * WARNING: An indication that something unexpected happened, and that user action may be required.
-* ERROR: An indication that a more serious issue has occurred, where something failed but the task is continuing.
+* ERROR: An indication that a more serious issue has occured, where something failed but the task is continuing.
 * CRITICAL: A serious error, indicating that the program itself may be unable to continue running.
 
 By default, all messages except for DEBUG messages are displayed. Messages can also be sent to a file and time stamped.
 
 See the :ref:`logger` documentation for instructions on how to control the verbosity of the logger.
 
 
@@ -379,15 +379,15 @@
 .. _whatsnew-1.0-moved-config:
 
 Config File Location Moved
 ==========================
 
 If you have customised your :ref:`customizing-with-sunpyrc-files` you will need to move it to the new config file location.
 Your old file should be in ``~/.sunpy/sunpyrc`` file and the new location, which is now platform specific, can be found by running `sunpy.print_config`.
-We recommend that your take a look at the new file as available configuration options have increased.
+We recommand that your take a look at the new file as available configuration options have increased.
 
 .. _whatsnew-1.0-renamed-removed:
 
 Renamed/removed functionality
 =============================
 
 This is just some of the renamed or removed functionality.
```

### Comparing `sunpy-4.1.5/docs/whatsnew/1.1-wispr.png` & `sunpy-4.1rc1/docs/whatsnew/1.1-wispr.png`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/1.1.rst` & `sunpy-4.1rc1/docs/whatsnew/1.1.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/2.0.rst` & `sunpy-4.1rc1/docs/whatsnew/2.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/2.1.rst` & `sunpy-4.1rc1/docs/whatsnew/2.1.rst`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
 .. _whatsnew-2.1-performance:
 
 Performance improvements
 ========================
 Several functions in `sunpy.map` have been significantly sped up with improved algorithms.
 
-In addition, `sunpy.map.GenericMap.wcs` is now cached when the map metadata remains unchanged, significantly improving performance in applications which make multiple requests for the map WCS (e.g. plotting), and reducing the number of repeated warnings thrown when metadata is missing.
+In addition, `sunpy.map.GenericMap.wcs` is now cached when the map metadata remains unchanged, significantly improving performance in applications which make mutiple requests for the map WCS (e.g. plotting), and reducing the number of repeated warnings thrown when metadata is missing.
 
 .. _whatsnew-2.1-python:
 
 Increase in required package versions
 =====================================
 We have bumped the minimum version of several packages we depend on; these are the new minimum versions for sunpy 2.1:
```

### Comparing `sunpy-4.1.5/docs/whatsnew/3.0.rst` & `sunpy-4.1rc1/docs/whatsnew/3.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/3.1.rst` & `sunpy-4.1rc1/docs/whatsnew/3.1.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/4.0.rst` & `sunpy-4.1rc1/docs/whatsnew/4.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/docs/whatsnew/4.1.rst` & `sunpy-4.1rc1/docs/whatsnew/4.1.rst`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 See the changelog for full details on what has changed.
 
 To harmonize different ``peek()`` and ``plot()`` signatures, all non-keyword arguments to these methods are deprecated.
 To avoid a warning pass all arguments with keywords (e.g. ``plot(title='my plot title')``) instead.
 
 Updated data downloader dependency
 ==================================
-The package that handles downloading data from remote sources, ``parfive``, has had a recent major release to version 2.0.
+The pacakge that handles downloading data from remote sources, ``parfive``, has had a recent major release to version 2.0.
 This new version comes with major usability improvements: removal of incomplete files and major error reporting upgrades.
 
 sunpy users are encouraged to upgrade ``parfive`` to benefit from these improvements.
 To upgrade you can use pip:
 
 .. code-block:: bash
```

### Comparing `sunpy-4.1.5/docs/whatsnew/index.rst` & `sunpy-4.1rc1/docs/whatsnew/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/acquiring_data/downloading_cutouts.py` & `sunpy-4.1rc1/examples/acquiring_data/downloading_cutouts.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/acquiring_data/fido_metadata_queries.py` & `sunpy-4.1rc1/examples/acquiring_data/fido_metadata_queries.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/acquiring_data/querying_the_GOES_event_list.py` & `sunpy-4.1rc1/examples/acquiring_data/querying_the_GOES_event_list.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/acquiring_data/search_cdaweb.py` & `sunpy-4.1rc1/examples/acquiring_data/search_cdaweb.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/acquiring_data/searching_vso.py` & `sunpy-4.1rc1/examples/acquiring_data/searching_vso.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/computer_vision_techniques/finding_masking_bright_pixels.py` & `sunpy-4.1rc1/examples/computer_vision_techniques/finding_masking_bright_pixels.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/computer_vision_techniques/loop_edge_enhance.py` & `sunpy-4.1rc1/examples/computer_vision_techniques/loop_edge_enhance.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/computer_vision_techniques/mask_disk.py` & `sunpy-4.1rc1/examples/computer_vision_techniques/mask_disk.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/computer_vision_techniques/off_limb_enhance.py` & `sunpy-4.1rc1/examples/computer_vision_techniques/off_limb_enhance.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/developer_tools/remote_data_manager.py` & `sunpy-4.1rc1/examples/developer_tools/remote_data_manager.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/differential_rotation/comparing_rotation_models.py` & `sunpy-4.1rc1/examples/differential_rotation/comparing_rotation_models.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/differential_rotation/differentially_rotated_coordinate.py` & `sunpy-4.1rc1/examples/differential_rotation/differentially_rotated_coordinate.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ##############################################################################
 # We can differentially rotate this coordinate by using
 # `~sunpy.coordinates.metaframes.RotatedSunFrame` with an array of observation
 # times.  Let's define a daily cadence for +/- five days.
 
 durations = np.concatenate([range(-5, 0), range(1, 6)]) * u.day
-diffrot_point = SkyCoord(RotatedSunFrame(base=point, duration=durations))
+diffrot_point = RotatedSunFrame(base=point, duration=durations)
 
 ##############################################################################
 # To see what this coordinate looks like in "real" helioprojective
 # Cartesian coordinates, we can transform it back to the original frame.
 # Since these coordinates are represented in the original frame, they will not
 # account for the changing position of the observer over this same time range.
```

### Comparing `sunpy-4.1.5/examples/differential_rotation/differentially_rotated_gridlines.py` & `sunpy-4.1rc1/examples/differential_rotation/differentially_rotated_gridlines.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/differential_rotation/reprojected_map.py` & `sunpy-4.1rc1/examples/differential_rotation/reprojected_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/example_template/example_template.py` & `sunpy-4.1rc1/examples/example_template/example_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # block. To include this new comment string we started the new block with a
 # long line of hashes.
 #
 # The sphinx-gallery parser will assume everything after this splitter and that
 # continues to start with a **comment hash and space** (respecting code style)
 # is text that has to be rendered in
 # html format. Keep in mind to always keep your comments always together by
-# comment hashes. That means to break a paragraph you still need to comment
+# comment hashes. That means to break a paragraph you still need to commend
 # that line break.
 #
 # In this example the next block of code produces some plotable data. Code is
 # executed, figure is saved and then code is presented next, followed by the
 # inlined figure.
 
 x = np.linspace(-np.pi, np.pi, 300)
```

### Comparing `sunpy-4.1.5/examples/map/brightness_pixel_location.py` & `sunpy-4.1rc1/examples/map/brightness_pixel_location.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/compare_rotation_results.py` & `sunpy-4.1rc1/examples/map/compare_rotation_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 scipy_map = hmi_map.rotate(method='scipy')
 skimage_map = hmi_map.rotate(method='scikit-image')
 cv2_map = hmi_map.rotate(method='opencv')
 
 ###############################################################################
 # Now for a visual comparison, the raw differences, that should highlight the differences.
-# Note that only two comparisons are shown.  Note the scale here is ± 10.
+# Note that only two comparisions are shown.  Note the scale here is ± 10.
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12, 6))
 
 img1 = ax1.imshow(scipy_map.data - skimage_map.data, cmap='RdBu_r', vmin=-10, vmax=10)
 ax1.set_title("HMI Difference: scipy vs scikit-image")
 fig.colorbar(img1, ax=ax1)
 
@@ -55,15 +55,15 @@
 
 scipy_map = aia_map.rotate(30*u.deg, method='scipy')
 skimage_map = aia_map.rotate(30*u.deg, method='scikit-image')
 cv2_map = aia_map.rotate(30*u.deg, method='opencv')
 
 ###############################################################################
 # Now for a visual comparison, the raw differences, that should highlight the differences.
-# Note that only two comparisons are shown. Note the scale here is ± 75.
+# Note that only two comparisions are shown. Note the scale here is ± 75.
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12, 6))
 
 img1 = ax1.imshow(scipy_map.data - skimage_map.data, cmap='RdBu_r', vmin=-75, vmax=75)
 ax1.set_title("AIA Difference: scipy vs scikit-image")
 fig.colorbar(img1, ax=ax1)
```

### Comparing `sunpy-4.1.5/examples/map/composite_map_AIA_HMI.py` & `sunpy-4.1rc1/examples/map/composite_map_AIA_HMI.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/difference_images.py` & `sunpy-4.1rc1/examples/map/difference_images.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/hmi_contours_wcsaxes.py` & `sunpy-4.1rc1/examples/map/hmi_contours_wcsaxes.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/image_bright_regions_gallery_example.py` & `sunpy-4.1rc1/examples/map/image_bright_regions_gallery_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/map_contouring.py` & `sunpy-4.1rc1/examples/map/map_contouring.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/map_data_histogram.py` & `sunpy-4.1rc1/examples/map/map_data_histogram.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/map_from_numpy_array.py` & `sunpy-4.1rc1/examples/map/map_from_numpy_array.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/map_metadata_modification.py` & `sunpy-4.1rc1/examples/map/map_metadata_modification.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/map_resampling_and_superpixels.py` & `sunpy-4.1rc1/examples/map/map_resampling_and_superpixels.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/map_rotation.py` & `sunpy-4.1rc1/examples/map/map_rotation.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/map_segment.py` & `sunpy-4.1rc1/examples/map/map_segment.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map/plot_frameless_image.py` & `sunpy-4.1rc1/examples/map/plot_frameless_image.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map_transformations/autoalign_aia_hmi.py` & `sunpy-4.1rc1/examples/map_transformations/autoalign_aia_hmi.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,26 +41,18 @@
 ax2 = fig.add_subplot(122, projection=map_hmi)
 map_hmi.plot(axes=ax2)
 
 ######################################################################
 # Setting ``autoalign=True`` allows plotting the HMI image onto axes
 # defined by the AIA reference frame.  In contrast to the above code
 # block, we intentionally set the ``projection`` for the axes to be
-# the AIA map instead of the HMI map. We also need to manually set
+# the AIA map # instead of the HMI map.  We also need to manually set
 # the plot limits because Matplotlib gets confused by the off-disk
-# parts of the image. The HMI image now has the same
+# parts of the image.  Note that the HMI image now has the same
 # orientation as the AIA image.
-#
-# Note that off-disk HMI data are not retained by default because an
-# additional assumption is required to define the location of the HMI
-# emission in 3D space. We can use
-# :meth:`~sunpy.coordinates.Helioprojective.assume_spherical_screen` to
-# retain the off-disk HMI data. See
-# :ref:`sphx_glr_generated_gallery_map_transformations_reprojection_spherical_screen.py`
-# for more reference.
 
 fig = plt.figure(figsize=(12, 5))
 ax1 = fig.add_subplot(121, projection=map_aia)
 map_aia.plot(axes=ax1, clip_interval=(1, 99.9)*u.percent)
 ax2 = fig.add_subplot(122, projection=map_aia)
 map_hmi.plot(axes=ax2, autoalign=True, title='HMI image in AIA reference frame')
 ax2.axis(ax1.axis())
```

### Comparing `sunpy-4.1.5/examples/map_transformations/projection_custom_origin.py` & `sunpy-4.1rc1/examples/map_transformations/projection_custom_origin.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map_transformations/reprojection_aia_euvi_mosaic.py` & `sunpy-4.1rc1/examples/map_transformations/reprojection_aia_euvi_mosaic.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map_transformations/reprojection_align_aia_hmi.py` & `sunpy-4.1rc1/examples/map_transformations/reprojection_align_aia_hmi.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,22 +51,14 @@
 # two WCSes with the same observer, which makes it well suited to aligning
 # data.
 
 out_hmi = map_hmi.reproject_to(map_aia.wcs)
 
 ######################################################################
 # Plot the images side by side.
-#
-# Note that off-disk HMI data are not retained by default because an
-# additional assumption is required to define the location of the HMI
-# emission in 3D space. We can use
-# :meth:`~sunpy.coordinates.Helioprojective.assume_spherical_screen` to
-# retain the off-disk HMI data. See
-# :ref:`sphx_glr_generated_gallery_map_transformations_reprojection_spherical_screen.py`
-# for more reference.
 
 fig = plt.figure(figsize=(12, 5))
 ax1 = fig.add_subplot(121, projection=map_aia)
 map_aia.plot(axes=ax1, clip_interval=(1, 99.9)*u.percent)
 ax2 = fig.add_subplot(122, projection=out_hmi)
 out_hmi.plot(axes=ax2, title='Reprojected HMI image')
```

### Comparing `sunpy-4.1.5/examples/map_transformations/reprojection_carrington.py` & `sunpy-4.1rc1/examples/map_transformations/reprojection_carrington.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map_transformations/reprojection_different_observers.py` & `sunpy-4.1rc1/examples/map_transformations/reprojection_different_observers.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map_transformations/reprojection_spherical_screen.py` & `sunpy-4.1rc1/examples/map_transformations/reprojection_spherical_screen.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/map_transformations/upside_down_hmi.py` & `sunpy-4.1rc1/examples/map_transformations/upside_down_hmi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ==============================================
 Rotating HMI maps so they're not 'upside-down'
 ==============================================
 
 This example shows how to rotate a HMI magnetogram, so when you plot it
-it appears with solar North pointing up.
+it appears with solar North puting up, and pointing up.
 """
 import matplotlib.pyplot as plt
 
 import sunpy.map
 from sunpy.data.sample import HMI_LOS_IMAGE
 
 ###############################################################################
```

### Comparing `sunpy-4.1.5/examples/plotting/aia_example.py` & `sunpy-4.1rc1/examples/plotting/aia_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/arrayanimatorwcs.py` & `sunpy-4.1rc1/examples/plotting/arrayanimatorwcs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/fading_between_maps.py` & `sunpy-4.1rc1/examples/plotting/fading_between_maps.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/finding_local_peaks_in_solar_data.py` & `sunpy-4.1rc1/examples/plotting/finding_local_peaks_in_solar_data.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/finegrained_plot.py` & `sunpy-4.1rc1/examples/plotting/finegrained_plot.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/great_arc_example.py` & `sunpy-4.1rc1/examples/plotting/great_arc_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/grid_plotting.py` & `sunpy-4.1rc1/examples/plotting/grid_plotting.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/hmi_cutout.py` & `sunpy-4.1rc1/examples/plotting/hmi_cutout.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/hmi_synoptic_maps.py` & `sunpy-4.1rc1/examples/plotting/hmi_synoptic_maps.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/lat_lon_lines.py` & `sunpy-4.1rc1/examples/plotting/lat_lon_lines.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 """
 =================================================
 Drawing heliographic longitude and latitude lines
 =================================================
 
-This example demonstrates how you can draw individual Stonyhurst
-longitude and latitude lines.
+How to draw your own (Stonyhurst) longitude and latitude lines.
 """
 import matplotlib.pyplot as plt
 import numpy as np
 
 import astropy.units as u
 from astropy.coordinates import SkyCoord
 
 import sunpy.map
 from sunpy.coordinates import frames
 from sunpy.data.sample import AIA_171_IMAGE
 
 ###############################################################################
-# We will first demonstrate the coordinate transformations that occur under the
-# hood to show a heliographic grid line of longitude or latitude.
-# Let's start with a map using the sample data.
+# The purpose of this example is to demonstrate the coordinate transformations
+# that occur under the hood to show the heliographic grid lines of longitude
+# latitude. We first create the Map using the sample data.
 
 aia = sunpy.map.Map(AIA_171_IMAGE)
 
 ###############################################################################
-# We can define a heliographic coordinate for a single point.
+# Let's first transform a single heliographic point coordinate.
 
-lon_value = 35 * u.deg
-lat_value = 12 * u.deg
-stonyhurst_frame = frames.HeliographicStonyhurst(obstime=aia.date)
-point_in_stonyhurst = SkyCoord(lon=lon_value, lat=lat_value, frame=stonyhurst_frame)
+stonyhurst_center = SkyCoord(12 * u.deg, 12 * u.deg,
+                             frame=frames.HeliographicStonyhurst)
 
 ###############################################################################
-# Next we transform it into the coordinate frame of our map, which is helioprojective.
+# Next we transform it into the coordinate frame of our map which is in
+# helioprojective coordinates.
 
-point_in_hpc = point_in_stonyhurst.transform_to(aia.coordinate_frame)
-print(point_in_hpc)
+hpc_stonyhurst_center = stonyhurst_center.transform_to(aia.coordinate_frame)
+print(hpc_stonyhurst_center)
 
 ###############################################################################
-# Now let's define two lines, one of constant longitude and one of constant latitude,
-# that pass through the previously defined coordinate point.
+# Now let's define two lines, one of longitude and one of of latitude.
 # We don't need to explicitly transform them to the coordinate frame of our
 # map because they will be transformed automatically when plotted.
 
 num_points = 100
-constant_lon = SkyCoord(lon_value, np.linspace(-90, 90, num_points) * u.deg,
-                        frame=stonyhurst_frame)
-constant_lat = SkyCoord(np.linspace(-90, 90, num_points) * u.deg, lat_value,
-                        frame=stonyhurst_frame)
+lat_value = 12 * u.deg
+lon_value = 35 * u.deg
+lon0 = SkyCoord(np.linspace(-80, 80, num_points) * u.deg,
+                np.ones(num_points) * lon_value, frame=frames.HeliographicStonyhurst)
+lat0 = SkyCoord(np.ones(num_points) * lat_value,
+                np.linspace(-90, 90, num_points) * u.deg,
+                frame=frames.HeliographicStonyhurst)
 
 ###############################################################################
-# Now let's plot the single coordinate point and the individual lines of
-# constant longitude and latitude. We'll overlay the autogenerated lon/lat
+# Now let's plot the results. We'll overlay the autogenerated lon/lat
 # grid as well for comparison.
 
 fig = plt.figure()
 ax = fig.add_subplot(projection=aia)
 aia.plot(axes=ax, clip_interval=(1, 99.99)*u.percent)
-ax.plot_coord(constant_lon, color="lightblue")
-ax.plot_coord(constant_lat, color="tomato")
-ax.plot_coord(point_in_stonyhurst, marker="o")
+ax.plot_coord(lat0, color="C0")
+ax.plot_coord(lon0, color="C0")
 aia.draw_grid(axes=ax)
 
 plt.show()
```

### Comparing `sunpy-4.1.5/examples/plotting/limb_plotting.py` & `sunpy-4.1rc1/examples/plotting/limb_plotting.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/lineAnimator_examples.py` & `sunpy-4.1rc1/examples/plotting/lineAnimator_examples.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/magnetogram_active_regions.py` & `sunpy-4.1rc1/examples/plotting/magnetogram_active_regions.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/map_editcolormap.py` & `sunpy-4.1rc1/examples/plotting/map_editcolormap.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/overplot_hek_polygon.py` & `sunpy-4.1rc1/examples/plotting/overplot_hek_polygon.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/plot_equator_prime_meridian.py` & `sunpy-4.1rc1/examples/plotting/plot_equator_prime_meridian.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/plot_rectangle.py` & `sunpy-4.1rc1/examples/plotting/plot_rectangle.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/plotting_blank_map.py` & `sunpy-4.1rc1/examples/plotting/plotting_blank_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/quadrangle.py` & `sunpy-4.1rc1/examples/plotting/quadrangle.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/simple_differential_rotation.py` & `sunpy-4.1rc1/examples/plotting/simple_differential_rotation.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/solar_cycle_example.py` & `sunpy-4.1rc1/examples/plotting/solar_cycle_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/sunpy_matplotlib_colormap.py` & `sunpy-4.1rc1/examples/plotting/sunpy_matplotlib_colormap.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/wcsaxes_map_example.py` & `sunpy-4.1rc1/examples/plotting/wcsaxes_map_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/wcsaxes_plotting_example.py` & `sunpy-4.1rc1/examples/plotting/wcsaxes_plotting_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/plotting/xy_lims.py` & `sunpy-4.1rc1/examples/plotting/xy_lims.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # coordinates these correspond to.
 # Lets choose x-limits and y-limits in arcsecs that we are interested in.
 
 xlims_world = [500, 1100]*u.arcsec
 ylims_world = [-800, 0]*u.arcsec
 
 ###############################################################################
-# We can then convert these into a SkyCoord which can be passed to :func:`~sunpy.map.GenericMap.world_to_pixel` to
+# We can then covert these into a SkyCoord which can be passed to :func:`~sunpy.map.GenericMap.world_to_pixel` to
 # determine which pixel coordinates these represent on the Map.
 
 world_coords = SkyCoord(Tx=xlims_world, Ty=ylims_world, frame=aia_map.coordinate_frame)
 pixel_coords = aia_map.world_to_pixel(world_coords)
 
 # we can then pull out the x and y values of these limits.
 xlims_pixel = pixel_coords.x.value
```

### Comparing `sunpy-4.1.5/examples/saving_and_loading_data/coordinates_in_asdf.py` & `sunpy-4.1rc1/examples/saving_and_loading_data/coordinates_in_asdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/saving_and_loading_data/genericmap_in_asdf.py` & `sunpy-4.1rc1/examples/saving_and_loading_data/genericmap_in_asdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/saving_and_loading_data/genericmap_in_fits.py` & `sunpy-4.1rc1/examples/saving_and_loading_data/genericmap_in_fits.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/time_series/goes_hek_m25.py` & `sunpy-4.1rc1/examples/time_series/goes_hek_m25.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/time_series/goes_xrs_example.py` & `sunpy-4.1rc1/examples/time_series/goes_xrs_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 # refer to the `GOES Data Guide <https://satdat.ngdc.noaa.gov/sem/goes/data/science/xrs/GOES_13-15_XRS_Science-Quality_Data_Readme.pdf>`__.
 
 df = goes_15.to_dataframe()
 df = df[(df["xrsa_quality"] == 0) & (df["xrsb_quality"] == 0)]
 goes_15 = ts.TimeSeries(df, goes_15.meta, goes_15.units)
 
 ###############################################################
-# We can also pull out the individual GOES channels and plot. The 0.5-4 angstrom
+# We can also pull out the individual GOES chanels and plot. The 0.5-4 angstrom
 # channel is known as the "xrsa" channel and the 1-8 angstrom channel is known
 # as the "xrsb" channel.
 
 goes_15.plot(columns=["xrsb"])
 plt.show()
 
 ###############################################################
```

### Comparing `sunpy-4.1.5/examples/time_series/power_spectra_example.py` & `sunpy-4.1rc1/examples/time_series/power_spectra_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # seconds.
 
 ts = sunpy.timeseries.TimeSeries(RHESSI_TIMESERIES)
 
 ###############################################################################
 # We now use SciPy's `~scipy.signal.periodogram` to estimate the
 # power spectra of the first column of the Timeseries. The first column contains
-# X-Ray emissions in the range of 3-6 keV. An alternative version is Astropy's
+# X-Ray emmisions in the range of 3-6 keV. An alternative version is Astropy's
 # `~astropy.timeseries.LombScargle` periodogram.
 
 x_ray = ts.columns[0]
 # The suitable value for fs would be 0.25 Hz as the time step is 4 s.
 freq, spectra = signal.periodogram(ts.quantity(x_ray), fs=0.25)
 
 ###############################################################################
```

### Comparing `sunpy-4.1.5/examples/time_series/timeseries_convolution_filter.py` & `sunpy-4.1rc1/examples/time_series/timeseries_convolution_filter.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/time_series/timeseries_example.py` & `sunpy-4.1rc1/examples/time_series/timeseries_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-================
-Using TimeSeries
-================
+====================================
+Using `~sunpy.timeseries.TimeSeries`
+====================================
 
 This example is intended to demonstrate the current state of `~sunpy.timeseries.TimeSeries`.
 """
 import datetime
 from collections import OrderedDict
 
 import matplotlib.pyplot as plt
@@ -20,17 +20,17 @@
 from sunpy.net import Fido
 from sunpy.net import attrs as a
 from sunpy.time import TimeRange, parse_time
 from sunpy.util.metadata import MetaDict
 
 ##############################################################################
 # We can create a range of supported timeseries:
+
 # There is a ``source`` keyword that allows one to specify the source of the data
 # It should be auto-detected in most cases.
-
 ts_eve = sunpy.timeseries.TimeSeries(sunpy.data.sample.EVE_TIMESERIES, source='EVE')
 ts_goes = sunpy.timeseries.TimeSeries(sunpy.data.sample.GOES_XRS_TIMESERIES, source='XRS')
 ts_lyra = sunpy.timeseries.TimeSeries(sunpy.data.sample.LYRA_LEVEL3_TIMESERIES, source='LYRA')
 ts_norh = sunpy.timeseries.TimeSeries(sunpy.data.sample.NORH_TIMESERIES, source='NoRH')
 ts_rhessi = sunpy.timeseries.TimeSeries(sunpy.data.sample.RHESSI_TIMESERIES, source='RHESSI')
 ts_gbm = sunpy.timeseries.TimeSeries(sunpy.data.sample.GBM_TIMESERIES, source='GBMSummary')
 
@@ -61,47 +61,51 @@
 # ``.data`` : The internal data representation. If you want the underlying data,
 # use `~sunpy.timeseries.GenericTimeSeries.to_dataframe()`
 # ``.meta`` : Stores the metadata that is able to be parsed from the data files
 # ``.units`` : Stores the units for each column, with keys that match the name of each column.
 
 # This will give you a useful dataframe to manipulate the data with.
 lyra_data = ts_lyra.to_dataframe()
-lyra_data
 
 ##############################################################################
 # This will give you the metadata
 ts_lyra.meta
 
 ##############################################################################
 # This will give you the units
 ts_lyra.units
 
 ##############################################################################
 # There are a couple of other useful properties:
 
-# The time range of the data, the name of the data columns
-ts_lyra.time_range, ts_lyra.columns
+# The time range of the data
+ts_lyra.time_range
+# The name of the data columns
+ts_lyra.columns
 
 ##############################################################################
 # Further data is available from within the metadata, you can filter out for a
 # key using the :meth:`.TimeSeriesMetaData.get` method.
 
-combined_goes_ts.meta.get("publisher_name")
+combined_goes_ts.meta.get('telescop')
+# This returns a `.TimeSeriesMetaData` object, if you want just a list values
+combined_goes_ts.meta.get('telescop').values()
 
 ##############################################################################
 # You can access a specific value within the `~sunpy.timeseries.TimeSeries` data
 # using all the normal `pandas` methods.
 # For example, to get the row with the index of "2015-01-01 00:02:00.008000"
 # Pandas will actually parse a string to a datetime automatically if it can:
 
 lyra_data.loc['2011-06-07 00:02:00.010']
 # If this fails, you will need to use parse_time to convert the string to a datetime
 lyra_data.loc[parse_time('2011-06-07 00:02:00.010').datetime]
 # Pandas includes methods to find the indexes of the max/min values in a dataframe:
-ts_lyra.to_dataframe()['CHANNEL1'].idxmax(), ts_lyra.to_dataframe()['CHANNEL1'].idxmin()
+ts_lyra.to_dataframe()['CHANNEL1'].idxmax()
+ts_lyra.to_dataframe()['CHANNEL1'].idxmin()
 
 ##############################################################################
 # An individual column can be extracted
 
 ts_eve.extract('CMLon')
 
 ##############################################################################
@@ -118,15 +122,16 @@
 
 ##############################################################################
 # You can add or overwrite a column using :meth:`sunpy.timeseries.GenericTimeSeries.add_column`.
 # This method only accepts an `~astropy.units.Quantity` and will convert to the intended units
 # if necessary.
 
 new_quantity = quantity.value * 0.01 * ts_eve.units[colname]
-new_eve_ts = ts_eve.add_column(colname, new_quantity, overwrite=True)
+new_quantity
+ts_eve.add_column(colname, new_quantity, overwrite=True)
 
 ##############################################################################
 # You can truncate using the :meth:`sunpy.timeseries.GenericTimeSeries.truncate` method.
 
 ts_goes_trunc = ts_goes.truncate(0, 100000, 2)
 # Or using a `TimeRange`
 ts_goes_trunc = ts_goes.truncate(TimeRange('2011-06-07 05:00', '2011-06-07 06:30'))
```

### Comparing `sunpy-4.1.5/examples/time_series/timeseries_peak_finding.py` & `sunpy-4.1rc1/examples/time_series/timeseries_peak_finding.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 
     Returns
     -------
     minpeaks, maxpeaks : `list`
         Lists consisting of pos, val pairs for both local minima points and
         local maxima points.
     """
-    # Set initial values
+    # Set inital values
     mn, mx = np.Inf, -np.Inf
     minpeaks = []
     maxpeaks = []
     lookformax = True
     start = True
     # Iterate over items in series
-    for time_pos, value in series.items():
+    for time_pos, value in series.iteritems():
         if value > mx:
             mx = value
             mxpos = time_pos
         if value < mn:
             mn = value
             mnpos = time_pos
         if lookformax:
@@ -94,18 +94,16 @@
     return minpeaks, maxpeaks
 
 
 ##############################################################################
 # Now we take the column 'sunspot SWO' of this TimeSeries and try to find it's
 # extrema using the function findpeaks. We take the value of DELTA to be
 # approximately the length of smallest peak that we wish to detect.
-
 series = my_timeseries.to_dataframe()['xrsa']
 minpeaks, maxpeaks = findpeaks(series, DELTA=1e-7)
-
 # Plotting the figure and extremum points
 plt.figure()
 plt.xlabel('Time')
 plt.ylabel("Flux (Wm$^{-2}$")
 plt.title('Peaks in TimeSeries')
 series.plot()
 plt.scatter(*zip(*minpeaks), color='red', label='min')
```

### Comparing `sunpy-4.1.5/examples/time_series/timeseriesmetadata_example.py` & `sunpy-4.1rc1/examples/time_series/timeseriesmetadata_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/AIA_limb_STEREO.py` & `sunpy-4.1rc1/examples/units_and_coordinates/AIA_limb_STEREO.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/AltAz_Coordinate_transform.py` & `sunpy-4.1rc1/examples/units_and_coordinates/AltAz_Coordinate_transform.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py` & `sunpy-4.1rc1/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/STEREO_SECCHI_starfield.py` & `sunpy-4.1rc1/examples/units_and_coordinates/STEREO_SECCHI_starfield.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/constants_reference.py` & `sunpy-4.1rc1/examples/units_and_coordinates/constants_reference.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/getting_lasco_observer_location.py` & `sunpy-4.1rc1/examples/units_and_coordinates/getting_lasco_observer_location.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/getting_observer_location.py` & `sunpy-4.1rc1/examples/units_and_coordinates/getting_observer_location.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/map_slit_extraction.py` & `sunpy-4.1rc1/examples/units_and_coordinates/map_slit_extraction.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/north_offset_frame.py` & `sunpy-4.1rc1/examples/units_and_coordinates/north_offset_frame.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/parse_time.py` & `sunpy-4.1rc1/examples/units_and_coordinates/parse_time.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/planet_locations.py` & `sunpy-4.1rc1/examples/units_and_coordinates/planet_locations.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/radec_to_hpc_map.py` & `sunpy-4.1rc1/examples/units_and_coordinates/radec_to_hpc_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/examples/units_and_coordinates/venus_transit.py` & `sunpy-4.1rc1/examples/units_and_coordinates/venus_transit.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/licenses/ASTROPY.rst` & `sunpy-4.1rc1/licenses/ASTROPY.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/licenses/GLUE.rst` & `sunpy-4.1rc1/licenses/GLUE.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/licenses/SCIKIT-LEARN.rst` & `sunpy-4.1rc1/licenses/SCIKIT-LEARN.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/licenses/TOWNCRIER.rst` & `sunpy-4.1rc1/licenses/TOWNCRIER.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/pyproject.toml` & `sunpy-4.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
          "extension-helpers"
          ]
 build-backend = 'setuptools.build_meta'
 
 # Until we have h5py binaries we can't test wheels on Python 3.11
 [tool.cibuildwheel]
 test-skip = "cp311-*"
-test-requires = ["opencv_python==4.6.0.66"]
 
 [ tool.gilesbot ]
   [ tool.gilesbot.circleci_artifacts ]
     enabled = true
 
   [ tool.gilesbot.circleci_artifacts.figure_report ]
     url = ".tmp/py310-figure/figure_test_images/fig_comparison.html"
```

### Comparing `sunpy-4.1.5/setup.cfg` & `sunpy-4.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -52,23 +52,23 @@
 	asdf>=2.8.0
 dask = 
 	dask[array]>=2.0.0
 database = 
 	sqlalchemy>=1.3.4
 image = 
 	scikit-image>=0.16.0
-	scipy>=1.3.0,!=1.10.0
+	scipy>=1.3.0
 jpeg2000 = 
 	glymur>=0.8.18,!=0.9.0,!=0.9.5
 	lxml>=4.8.0
 map = 
 	matplotlib>=3.3.0
 	mpl-animators>=1.0.0
 	reproject
-	scipy>=1.3.0,!=1.10.0
+	scipy>=1.3.0
 net = 
 	beautifulsoup4>=4.8.0
 	drms>=0.6.1
 	python-dateutil>=2.8.0
 	tqdm>=4.32.1
 	zeep>=3.4.0
 timeseries = 
@@ -100,19 +100,17 @@
 	reproject
 	ruamel.yaml
 	sphinx
 	sphinx-automodapi
 	sphinx-changelog>=1.1.1 # First to support towncrier 21.3
 	sphinx-copybutton
 	sphinx-design
-	sphinx-gallery>=0.11.1 # First to fix https://github.com/sunpy/sunpy/issues/6377
+	sphinx-gallery>=0.9.0 # First to include the defer figures functionality
 	sphinxext-opengraph
-	sunkit_image
 	sunpy-sphinx-theme
-	towncrier<22.12.0
 
 [options.packages.find]
 exclude = sunpy._dev
 
 [options.entry_points]
 asdf.resource_mappings = 
 	sunpy = sunpy.io.special.asdf.entry_points:get_resource_mappings
@@ -140,15 +138,14 @@
 	array_compare
 remote_data_strict = True
 junit_family = xunit1
 filterwarnings = 
 	error
 	always::pytest.PytestConfigWarning
 	ignore:The sunpy.database module is no longer actively maintained
-	ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning
 	ignore:Unknown pytest.mark.xdist_group
 	ignore:distutils Version classes are deprecated
 	ignore:numpy.ufunc size changed:RuntimeWarning
 	ignore:numpy.ndarray size changed:RuntimeWarning
 	ignore:defusedxml.lxml is no longer supported:DeprecationWarning
 	ignore:Distutils was imported before Setuptools
 	ignore:Matplotlib is currently using agg, which is a non-GUI backend, so cannot show the figure.
@@ -162,17 +159,14 @@
 	ignore:invalid value encountered in greater:RuntimeWarning
 	ignore:invalid value encountered in less:RuntimeWarning
 	ignore:FLIP_TOP_BOTTOM is deprecated and will be removed in Pillow 10:DeprecationWarning
 	ignore:Starting with ImageIO v3 the behavior of this function will switch:DeprecationWarning
 	ignore:unable to download valid IERS file, using local IERS-B
 	ignore:.*will attempt to set the values inplace instead of always setting a new array:FutureWarning
 	ignore:'cgi' is deprecated and slated for removal in Python 3.13:DeprecationWarning:zeep.utils
-	ignore:.*np.bool8.*is a deprecated alias.*:DeprecationWarning
-	ignore:Deprecated API features detected.*SQLAlchemy 2
-	ignore:`product` is deprecated as of NumPy 1.25.0:DeprecationWarning
 
 [pycodestyle]
 max_line_length = 110
 
 [flake8]
 max-line-length = 110
 exclude = 
@@ -227,22 +221,11 @@
 	pragma: no cover
 	except ImportError
 	raise AssertionError
 	raise NotImplementedError
 	def main\(.*\):
 	pragma: py{ignore_python_version}
 
-[codespell]
-skip = *.asdf,*.fits,*.fts,*.header,*.json,*.xsh,*cache*,*egg*,*extern*,.git,.idea,.tox,_build,*truncated
-ignore-words-list = 
-	alog,
-	nd,
-	nin,
-	observ,
-	ot,
-	te,
-	upto
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sunpy-4.1.5/setup.py` & `sunpy-4.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/CITATION.rst` & `sunpy-4.1rc1/sunpy/CITATION.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/__init__.py` & `sunpy-4.1rc1/sunpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/_compiler.c` & `sunpy-4.1rc1/sunpy/_compiler.c`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/conftest.py` & `sunpy-4.1rc1/sunpy/conftest.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/__init__.py` & `sunpy-4.1rc1/sunpy/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/ephemeris.py` & `sunpy-4.1rc1/sunpy/coordinates/ephemeris.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/frameattributes.py` & `sunpy-4.1rc1/sunpy/coordinates/frameattributes.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/frames.py` & `sunpy-4.1rc1/sunpy/coordinates/frames.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/metaframes.py` & `sunpy-4.1rc1/sunpy/coordinates/metaframes.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/offset_frame.py` & `sunpy-4.1rc1/sunpy/coordinates/offset_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     A frame which is offset from another frame such that it shares the same origin, but has its
     "north pole" (i.e., the Z axis) in a different direction.
 
     The original coordinate frame and the direction of the new north pole are specified by the
     ``north`` keyword.
 
-    This class should be used when specifying a new north pole is natural.  In contrast, for
+    This class should be used when specifying a new north pole is natural.  In constrast, for
     shifting the origin in the projected sky (e.g., where helioprojective X and Y coordinates are
     zero), use `~astropy.coordinates.SkyOffsetFrame` instead.
 
     Parameters
     ----------
     north : `~sunpy.coordinates.frames.HeliographicStonyhurst`
         The direction and frame for the new "north pole".
```

### Comparing `sunpy-4.1.5/sunpy/coordinates/sun.py` & `sunpy-4.1rc1/sunpy/coordinates/sun.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         lon = true_longitude(t)
         lat = true_latitude(t)
 
         # See Astronomical Algorithms (Meeus 1998 p.93)
         result = np.arcsin(np.sin(lat) * np.cos(obl) + np.cos(lat) * np.sin(obl) * np.sin(lon))
     else:
         # J2000.0 epoch
-        # Calculate Earth's true geometric declination relative to the Sun and multiply by -1.
+        # Calculate Earth's true geometric declination relative to the Sun and multipy by -1.
         # This approach is used because Astropy's GCRS includes aberration.
         earth = SkyCoord(0*u.deg, 0*u.deg, 0*u.AU, frame='gcrs', obstime=parse_time(t))
         result = -earth.hcrs.dec
 
     return Latitude(result, u.deg)
```

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/strategies.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_ephemeris.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_ephemeris.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_frameattributes.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_frameattributes.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_frames.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_metaframes.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_metaframes.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_offset_frame.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_offset_frame.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_sun.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_sun.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_transformations.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from sunpy.sun.constants import sidereal_rotation_rate
 from sunpy.time import parse_time
 
 
 def test_hcc_to_hgs():
     '''
     Check that a coordinate pointing to the observer in Heliocentric
-    coordinates maps to the latitude/longitude of the observer in
+    coordinates maps to the lattitude/longitude of the observer in
     HeliographicStonyhurst coordinates.
     '''
     lat = 10 * u.deg
     lon = 20 * u.deg
     observer = HeliographicStonyhurst(lat=lat, lon=lon)
     hcc_in = Heliocentric(x=0*u.km, y=0*u.km, z=1*u.km, observer=observer)
     hgs_out = hcc_in.transform_to(HeliographicStonyhurst())
```

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_utils.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     get_limb_coordinates,
     get_rectangle_coordinates,
     solar_angle_equivalency,
 )
 from sunpy.sun import constants
 
 # Test the great arc code against calculable quantities
-# The inner angle is the same between each pair of coordinates.  You can
-# calculate these coordinates using the inner angle formulae as listed here:
+# The inner angle is the same between each pair of co-ordinates.  You can
+# calculate these co-ordinates using the inner angle formulae as listed here:
 # https://en.wikipedia.org/wiki/Great-circle_distance
 
 
 @pytest.mark.parametrize("start, end", [((0, 0), (0, 45)),
                                         ((0, 0), (45, 0)),
                                         ((0, 45), (0, 0)),
                                         ((45, 0), (0, 0)),
```

### Comparing `sunpy-4.1.5/sunpy/coordinates/tests/test_wcs_utils.py` & `sunpy-4.1rc1/sunpy/coordinates/tests/test_wcs_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     assert_quantity_allclose(result.observer.lon, hgs_obs.lon)
     assert_quantity_allclose(result.observer.lat, hgs_obs.lat)
     assert_quantity_allclose(result.observer.radius, hgs_obs.radius)
 
 
 def test_wcs_aux():
     """
-    Make sure auxiliary information round trips properly from coordinate frames
+    Make sure auxillary information round trips properly from coordinate frames
     to WCS and back.
     """
     data = np.ones([6, 6], dtype=np.float64)
     header = {'CRVAL1': 0,
               'CRVAL2': 0,
               'CRPIX1': 5,
               'CRPIX2': 5,
```

### Comparing `sunpy-4.1.5/sunpy/coordinates/transformations.py` & `sunpy-4.1rc1/sunpy/coordinates/transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,40 +239,40 @@
         def wrapped_func(*args, **kwargs):
             global _layer_level
 
             # Check if the logging level is at least DEBUG (for performance reasons)
             debug_output = log.getEffectiveLevel() <= logging.DEBUG
 
             if debug_output:
-                # Indentation for transformation layer
-                indentation = u"\u2502   " * _layer_level
+                # Indention for transformation layer
+                indention = u"\u2502   " * _layer_level
 
-                # For the input arguments, add indentation to any lines after the first line
-                from_str = str(args[0]).replace("\n", f"\n       {indentation}\u2502       ")
-                to_str = str(args[1]).replace("\n", f"\n       {indentation}\u2502       ")
+                # For the input arguments, add indention to any lines after the first line
+                from_str = str(args[0]).replace("\n", f"\n       {indention}\u2502       ")
+                to_str = str(args[1]).replace("\n", f"\n       {indention}\u2502       ")
 
                 # Log the description and the input arguments
-                log.debug(f"{indentation}{description}")
-                log.debug(f"{indentation}\u251c\u2500From: {from_str}")
-                log.debug(f"{indentation}\u251c\u2500To  : {to_str}")
+                log.debug(f"{indention}{description}")
+                log.debug(f"{indention}\u251c\u2500From: {from_str}")
+                log.debug(f"{indention}\u251c\u2500To  : {to_str}")
 
-                # Increment the layer level to increase the indentation for nested transformations
+                # Increment the layer level to increase the indention for nested transformations
                 _layer_level += 1
 
             result = func(*args, **kwargs)
 
             if debug_output:
                 # Decrement the layer level
                 _layer_level -= 1
 
                 # For the output, add intention to any lines after the first line
-                out_str = str(result).replace("\n", f"\n       {indentation}        ")
+                out_str = str(result).replace("\n", f"\n       {indention}        ")
 
                 # Log the output
-                log.debug(f"{indentation}\u2514\u2500Out : {out_str}")
+                log.debug(f"{indention}\u2514\u2500Out : {out_str}")
 
             return result
         return wrapped_func
     return decorator
 
 
 def _observers_are_equal(obs_1, obs_2):
```

### Comparing `sunpy-4.1.5/sunpy/coordinates/utils.py` & `sunpy-4.1rc1/sunpy/coordinates/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,24 @@
         a GreatArc object sets the locations of the default points along the
         great arc.
 
     Methods
     -------
     inner_angles : `~astropy.units.Quantity`
         Angles of the points along the great arc from the start to end
-        coordinate.
+        co-ordinate.
 
     distances : `~astropy.units.Quantity`
         Distances of the points along the great arc from the start to end
-        coordinate.  The units are defined as those returned after transforming
-        the coordinate system of the start coordinate into its Cartesian
+        co-ordinate.  The units are defined as those returned after transforming
+        the co-ordinate system of the start co-ordinate into its Cartesian
         equivalent.
 
     coordinates : `~astropy.coordinates.SkyCoord`
-        Coordinates along the great arc in the coordinate frame of the
+        Co-ordinates along the great arc in the co-ordinate frame of the
         start point.
 
     References
     ----------
     [1] https://www.mathworks.com/matlabcentral/newsreader/view_thread/277881
     [2] https://en.wikipedia.org/wiki/Great-circle_distance#Vector_version
 
@@ -84,15 +84,15 @@
     """
 
     def __init__(self, start, end, center=None, points=None):
 
         # Observer
         self.observer = start.observer
 
-        # Coordinate frame of the starting point
+        # Co-ordinate frame of the starting point
         self.start_frame = start.frame
 
         # Observation time
         self.obstime = start.obstime
 
         # Start point of the great arc
         self.start = start.transform_to(Heliocentric)
@@ -171,15 +171,15 @@
             return points
         else:
             raise ValueError('Incorrectly specified "points" keyword value.')
 
     def inner_angles(self, points=None):
         """
         Calculates the inner angles for the parameterized points along the arc
-        and returns the value in radians, from the start coordinate to the
+        and returns the value in radians, from the start co-ordinate to the
         end.
 
         Parameters
         ----------
         points : `None`, `int`, `numpy.ndarray`
             If None, use the default locations of parameterized points along the
             arc.  If int, the arc is calculated at "points" equally spaced
@@ -189,24 +189,24 @@
             zero, denoting the start of the arc, to 1, denoting the end of the
             arc.
 
         Returns
         -------
         inner_angles : `~astropy.units.Quantity`
             Angles of the points along the great arc from the start to
-            end coordinate.
+            end co-ordinate.
 
         """
         these_points = self._points_handler(points)
         return these_points.reshape(len(these_points), 1)*self.inner_angle
 
     def distances(self, points=None):
         """
-        Calculates the distance from the start coordinate to the end
-        coordinate on the sphere for all the parameterized points.
+        Calculates the distance from the start co-ordinate to the end
+        co-ordinate on the sphere for all the parameterized points.
 
         Parameters
         ----------
         points : `None`, `int`, `numpy.ndarray`
             If None, use the default locations of parameterized points along the
             arc.  If int, the arc is calculated at "points" equally spaced
             points from start to end.  If a numpy.ndarray is passed, it must be
@@ -215,24 +215,24 @@
             zero, denoting the start of the arc, to 1, denoting the end of the
             arc.
 
         Returns
         -------
         distances : `~astropy.units`
             Distances of the points along the great arc from the start to end
-            coordinate.  The units are defined as those returned after
-            transforming the coordinate system of the start coordinate into
+            co-ordinate.  The units are defined as those returned after
+            transforming the co-ordinate system of the start co-ordinate into
             its Cartesian equivalent.
         """
         return self.radius * self.inner_angles(points=points).value
 
     def coordinates(self, points=None):
         """
-        Calculates the coordinates on the sphere from the start to the end
-        coordinate for all the parameterized points.  Coordinates are
+        Calculates the co-ordinates on the sphere from the start to the end
+        co-ordinate for all the parameterized points.  Co-ordinates are
         returned in the frame of the start coordinate.
 
         Parameters
         ----------
         points : `None`, `int`, `numpy.ndarray`
             If None, use the default locations of parameterized points along the
             arc.  If int, the arc is calculated at "points" equally spaced
@@ -241,15 +241,15 @@
             array correspond to parameterized locations along the great arc from
             zero, denoting the start of the arc, to 1, denoting the end of the
             arc.
 
         Returns
         -------
         arc : `~astropy.coordinates.SkyCoord`
-            Coordinates along the great arc in the coordinate frame of the
+            Co-ordinates along the great arc in the co-ordinate frame of the
             start point.
 
         """
         # Calculate the inner angles
         these_inner_angles = self.inner_angles(points=points)
 
         # Calculate the Cartesian locations from the first to second points
```

### Comparing `sunpy-4.1.5/sunpy/coordinates/wcs_utils.py` & `sunpy-4.1rc1/sunpy/coordinates/wcs_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         Parameters
         ----------
         obsgeo : array-like
             A shape ``(6, )`` array representing ``OBSGEO-[XYZ], OBSGEO-[BLH]`` as
             returned by ``WCS.wcs.obsgeo``.
         obstime : time-like
-            The time associated with the coordinate, will be passed to
+            The time assiociated with the coordinate, will be passed to
             `~.builtin_frames.ITRS` as the obstime keyword.
 
         Returns
         -------
         `~.builtin_frames.ITRS`
             An `~.builtin_frames.ITRS` coordinate frame
             representing the coordinates.
@@ -96,19 +96,19 @@
     """
 
     if hasattr(wcs, "coordinate_frame"):
         return wcs.coordinate_frame
 
     dateobs = wcs.wcs.dateobs or None
 
-    # Get observer coordinate from the WCS auxiliary information
+    # Get observer coordinate from the WCS auxillary information
     required_attrs = {HeliographicStonyhurst: ['hgln_obs', 'hglt_obs', 'dsun_obs'],
                       HeliographicCarrington: ['crln_obs', 'hglt_obs', 'dsun_obs']}
 
-    # Get rsun from the WCS auxiliary information
+    # Get rsun from the WCS auxillary information
     rsun = wcs.wcs.aux.rsun_ref
     if rsun is not None:
         rsun *= u.m
 
     # TODO: remove these errors in sunpy 4.1
     bad_attrs = [f'.{attr}' for attr in ['rsun', 'heliographic_observer']
                  if hasattr(wcs, attr)]
```

### Comparing `sunpy-4.1.5/sunpy/data/__init__.py` & `sunpy-4.1rc1/sunpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/_sample.py` & `sunpy-4.1rc1/sunpy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/cache.py` & `sunpy-4.1rc1/sunpy/data/data_manager/cache.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/downloader.py` & `sunpy-4.1rc1/sunpy/data/data_manager/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,12 +44,10 @@
     def download(self, url, path):
         downloader = Downloader()
         path = Path(path)
         filename = path.name
         directory = path.parent
         downloader.enqueue_file(url, directory, filename)
         try:
-            output = downloader.download()
+            downloader.download()
         except Exception as e:
             raise DownloaderError from e
-        if output.errors:
-            raise DownloaderError(output.errors[0].exception)
```

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/manager.py` & `sunpy-4.1rc1/sunpy/data/data_manager/manager.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/storage.py` & `sunpy-4.1rc1/sunpy/data/data_manager/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class StorageProviderBase(metaclass=ABCMeta):
     """
     Base class for remote data manager storage providers.
     """
     @abstractmethod
     def find_by_key(self, key, value):
         """
-        Returns the file details if value corresponding to the key
+        Returns the file details if value coresponding to the key
         found in storage. Returns `None` if hash not found.
 
         Parameters
         ----------
         key : `str`
             The key/column name of the field.
         value : `str`
@@ -133,15 +133,15 @@
     def connection(self, commit=False):
         """
         A context manager which provides an easy way to handle db connections.
 
         Parameters
         ----------
         commit : `bool`
-            Whether to commit after successful execution of db command.
+            Whether to commit after succesful execution of db command.
         """
         conn = sqlite3.connect(str(self._db_path))
         self._create_table(conn)
         try:
             yield conn
             if commit:
                 conn.commit()
```

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/tests/conftest.py` & `sunpy-4.1rc1/sunpy/data/data_manager/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/tests/mocks.py` & `sunpy-4.1rc1/sunpy/data/data_manager/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/tests/test_cache.py` & `sunpy-4.1rc1/sunpy/data/data_manager/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/tests/test_manager.py` & `sunpy-4.1rc1/sunpy/data/data_manager/tests/test_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
         # Storage still contains original test_file
         assert Path(storage._store[0]['file_path']).name == 'fake_module.test_file'
 
     # Request the original file again
     data_function_from_fake_module()
 
-    # File doesn't get redownloaded, instead it is retrieved using the file hash
+    # File dosn't get redownloaded, instead it is retrieved using the file hash
     assert downloader.times_called == 2
 
     # new_file entry in manager._file_cache is replaced with the original test_file
     assert Path(
         module_patched_manager._file_cache['test_file']['fake_module.']
     ).name == 'fake_module.test_file'
```

### Comparing `sunpy-4.1.5/sunpy/data/data_manager/tests/test_storage.py` & `sunpy-4.1rc1/sunpy/data/data_manager/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/sample.py` & `sunpy-4.1rc1/sunpy/data/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
    :header-rows: 1
 
    * - Sample shortname
      - Name of downloaded file
 """
 # download_sample_data is deprecated and not used here,
 # but during deprecation period want to keep it in this namespace
-# for backwards compatibility. noqa stops it being removed by
+# for backwards compatability. noqa stops it being removed by
 # pre-commit as an unused import
 from ._sample import download_sample_data  # noqa
 from ._sample import _SAMPLE_DATA, _get_sample_files
 
 # Add a table row to the module docstring for each sample file
 for _keyname, _filename in sorted(_SAMPLE_DATA.items()):
     __doc__ += f'   * - ``{_keyname}``\n     - {_filename}\n'
```

### Comparing `sunpy-4.1.5/sunpy/data/sunpyrc` & `sunpy-4.1rc1/sunpy/data/sunpyrc`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/20100621SRS.txt` & `sunpy-4.1rc1/sunpy/data/test/20100621SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/20150101SRS.txt` & `sunpy-4.1rc1/sunpy/data/test/20150101SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/20150306SRS.txt` & `sunpy-4.1rc1/sunpy/data/test/20150306SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/20150906SRS.txt` & `sunpy-4.1rc1/sunpy/data/test/20150906SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/20181209_180305_kcor_l2.header` & `sunpy-4.1rc1/sunpy/data/test/20181209_180305_kcor_l2.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT/efz20040301.000010_s.fits` & `sunpy-4.1rc1/sunpy/data/test/EIT/efz20040301.000010_s.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT/efz20040301.010016_s.fits` & `sunpy-4.1rc1/sunpy/data/test/EIT/efz20040301.010016_s.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.000010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.000010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.010016_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.010016_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.020010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.020010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.030011_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.030011_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.040010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.040010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.050010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.050010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.060010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.060010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.070014_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.070014_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.080010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.080010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.090010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.090010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.100010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.100010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.110010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.110010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EIT_header/efz20040301.120010_s.header` & `sunpy-4.1rc1/sunpy/data/test/EIT_header/efz20040301.120010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt` & `sunpy-4.1rc1/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/FGMG4_20110214_030443.7.header` & `sunpy-4.1rc1/sunpy/data/test/FGMG4_20110214_030443.7.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/HinodeSOT.header` & `sunpy-4.1rc1/sunpy/data/test/HinodeSOT.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/HinodeXRT.header` & `sunpy-4.1rc1/sunpy/data/test/HinodeXRT.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/SWAP/resampled0_swap.header` & `sunpy-4.1rc1/sunpy/data/test/SWAP/resampled0_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/SWAP/resampled1_swap.header` & `sunpy-4.1rc1/sunpy/data/test/SWAP/resampled1_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/SWAP/resampled2_swap.header` & `sunpy-4.1rc1/sunpy/data/test/SWAP/resampled2_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/SWAP/resampled3_swap.header` & `sunpy-4.1rc1/sunpy/data/test/SWAP/resampled3_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/YohkohSXT.header` & `sunpy-4.1rc1/sunpy/data/test/YohkohSXT.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/__init__.py` & `sunpy-4.1rc1/sunpy/data/test/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import numpy as np
 
 import astropy.io.fits
 from astropy.utils.data import get_pkg_data_filename
 
 import sunpy
-import sunpy.io._fits as _fits
 import sunpy.map
 
 __all__ = [
     'rootdir',
     'file_list',
     'get_test_filepath',
     'get_test_data_filenames',
@@ -107,16 +106,16 @@
     """
     Generate a dummy `~sunpy.map.Map` from header-only test data.
 
     The "image" will be random numbers with the correct shape
     as specified by the header.
     """
     filepath = get_test_filepath(filename)
-    header = _fits.format_comments_and_history(astropy.io.fits.Header.fromtextfile(filepath))
-    data = np.random.rand(header['NAXIS2'], header['NAXIS1'])
+    header = astropy.io.fits.Header.fromtextfile(filepath)
+    data = np.random.rand(header['naxis2'], header['naxis1'])
     if 'BITPIX' in header:
         data = data.astype(astropy.io.fits.BITPIX2DTYPE[header['BITPIX']])
     # NOTE: by reading straight from the data header pair, we are skipping
     # the fixes that are applied in sunpy.io._fits, e.g. the waveunit fix
     # Would it be better to write this whole map back to a temporary file and then
     # read it back in by passing in the filename instead?
     return sunpy.map.Map(data, header)
```

### Comparing `sunpy-4.1.5/sunpy/data/test/_generate_asdf_test.py` & `sunpy-4.1rc1/sunpy/data/test/_generate_asdf_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
 
 if __name__ == "__main__":
     import sunpy.map
     test_map = rootdir / "aia_171_level1.fits"
     obj = sunpy.map.Map(test_map)
     obj = obj.resample((2, 2)*u.pix)
-    # obj = obj.shift(10*u.arcsec, 0*u.arcsec)
+    #obj = obj.shift(10*u.arcsec, 0*u.arcsec)
     generate_asdf_tree(obj, "aiamap_genericmap_1.0.0.asdf")
```

### Comparing `sunpy-4.1.5/sunpy/data/test/aia_171_level1.fits` & `sunpy-4.1rc1/sunpy/data/test/aia_171_level1.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/aiamap_genericmap_1.0.0.asdf` & `sunpy-4.1rc1/sunpy/data/test/aiamap_genericmap_1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf` & `sunpy-4.1rc1/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/annotation_ppt.db` & `sunpy-4.1rc1/sunpy/data/test/annotation_ppt.db`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/cor1_20090615_000500_s4c1A.header` & `sunpy-4.1rc1/sunpy/data/test/cor1_20090615_000500_s4c1A.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header` & `sunpy-4.1rc1/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/euvi_20090615_000900_n4euA_s.header` & `sunpy-4.1rc1/sunpy/data/test/euvi_20090615_000900_n4euA_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/eve/eve_01.txt` & `sunpy-4.1rc1/sunpy/data/test/eve/eve_01.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/eve/eve_02.txt` & `sunpy-4.1rc1/sunpy/data/test/eve/eve_02.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/eve/eve_03.txt` & `sunpy-4.1rc1/sunpy/data/test/eve/eve_03.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/eve/eve_04.txt` & `sunpy-4.1rc1/sunpy/data/test/eve/eve_04.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/eve/eve_05.txt` & `sunpy-4.1rc1/sunpy/data/test/eve/eve_05.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits` & `sunpy-4.1rc1/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/gbm.fits` & `sunpy-4.1rc1/sunpy/data/test/gbm.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/generated_sample.genx` & `sunpy-4.1rc1/sunpy/data/test/generated_sample.genx`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/go1520110607.fits` & `sunpy-4.1rc1/sunpy/data/test/go1520110607.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/go1520120601.fits.gz` & `sunpy-4.1rc1/sunpy/data/test/go1520120601.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/goes_13_leap_second.nc` & `sunpy-4.1rc1/sunpy/data/test/goes_13_leap_second.nc`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/heliographic_phase_map.fits.gz` & `sunpy-4.1rc1/sunpy/data/test/heliographic_phase_map.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/hi_20110910_114721_s7h2A.header` & `sunpy-4.1rc1/sunpy/data/test/hi_20110910_114721_s7h2A.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/hmi_synoptic.header` & `sunpy-4.1rc1/sunpy/data/test/hmi_synoptic.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/hsi_image_20101016_191218.fits` & `sunpy-4.1rc1/sunpy/data/test/hsi_image_20101016_191218.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz` & `sunpy-4.1rc1/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header` & `sunpy-4.1rc1/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/lasco_c2_25299383_s.header` & `sunpy-4.1rc1/sunpy/data/test/lasco_c2_25299383_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/lasco_c3.header` & `sunpy-4.1rc1/sunpy/data/test/lasco_c3.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz` & `sunpy-4.1rc1/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header` & `sunpy-4.1rc1/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header` & `sunpy-4.1rc1/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/mdi_synoptic.header` & `sunpy-4.1rc1/sunpy/data/test/mdi_synoptic.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/observed-solar-cycle-indices-truncated.json` & `sunpy-4.1rc1/sunpy/data/test/observed-solar-cycle-indices-truncated.json`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/predicted-solar-cycle-truncated.json` & `sunpy-4.1rc1/sunpy/data/test/predicted-solar-cycle-truncated.json`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `sunpy-4.1rc1/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/resampled_hmi.fits` & `sunpy-4.1rc1/sunpy/data/test/resampled_hmi.fits`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc` & `sunpy-4.1rc1/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc` & `sunpy-4.1rc1/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc` & `sunpy-4.1rc1/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc` & `sunpy-4.1rc1/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc` & `sunpy-4.1rc1/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header` & `sunpy-4.1rc1/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf` & `sunpy-4.1rc1/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf` & `sunpy-4.1rc1/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/swap_lv1_20140606_000113.header` & `sunpy-4.1rc1/sunpy/data/test/swap_lv1_20140606_000113.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/tca110810_truncated` & `sunpy-4.1rc1/sunpy/data/test/tca110810_truncated`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/test_ana.fz` & `sunpy-4.1rc1/sunpy/data/test/test_ana.fz`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/tsi20010130_025823_a2.header` & `sunpy-4.1rc1/sunpy/data/test/tsi20010130_025823_a2.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header` & `sunpy-4.1rc1/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/waveunit/mq130812.084253.header` & `sunpy-4.1rc1/sunpy/data/test/waveunit/mq130812.084253.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/waveunit/na120701.091058.header` & `sunpy-4.1rc1/sunpy/data/test/waveunit/na120701.091058.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header` & `sunpy-4.1rc1/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/data/tests/test_sample.py` & `sunpy-4.1rc1/sunpy/data/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/__init__.py` & `sunpy-4.1rc1/sunpy/database/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/attrs.py` & `sunpy-4.1rc1/sunpy/database/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/caching.py` & `sunpy-4.1rc1/sunpy/database/caching.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/commands.py` & `sunpy-4.1rc1/sunpy/database/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 from abc import ABC, abstractmethod
 
 from sqlalchemy.exc import InvalidRequestError
 from sqlalchemy.orm import make_transient
 
-from sunpy.database.tables import DatabaseEntry
-
 __all__ = [
     'EmptyCommandStackError', 'NoSuchEntryError', 'NonRemovableTagError',
     'DatabaseOperation', 'AddEntry', 'RemoveEntry', 'EditEntry',
     'CommandManager']
 
 
 class EmptyCommandStackError(Exception):
@@ -92,28 +90,16 @@
             f = open(os.devnull, 'w')
             f.write(repr(operation))
             f.flush()
             f.close()
             operation()
 
     def undo(self):
-        # To prevent errors in SQLa 2.0 we have to first add all removed entries back in before we add any ~database.Tags.
-        for operation in self._operations:
-            if isinstance(operation, RemoveEntry):
-                # we also filter out ~database.commands.RemoveEntry where type is not ~database.tables.DatabaseEntry to do later.
-                if isinstance(operation.entry, DatabaseEntry):
-                    operation.undo()
         for operation in self._operations:
-            if isinstance(operation, RemoveEntry):
-                if not isinstance(operation.entry, DatabaseEntry):
-                    # undo all ~database.commands.RemoveEntry where type is not ~database.tables.DatabaseEntry
-                    operation.undo()
-            else:
-                # and we also undo all other commands, e.g. ~database.commands.RemoveTag.
-                operation.undo()
+            operation.undo()
 
     def __len__(self):
         return len(self._operations)
 
 
 class AddEntry(DatabaseOperation):
     """
```

### Comparing `sunpy-4.1.5/sunpy/database/database.py` & `sunpy-4.1rc1/sunpy/database/database.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/tables.py` & `sunpy-4.1rc1/sunpy/database/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # the Google Summer of Code (2013).
 import os
 import fnmatch
 from datetime import datetime
 
 import numpy as np
 from sqlalchemy import Boolean, Column, DateTime, Float, ForeignKey, Integer, String, Table
-from sqlalchemy.orm import declarative_base, relationship
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import relationship
 
 import astropy.table
 import astropy.units as u
 from astropy.time import Time
 from astropy.units import equivalencies
 
 import sunpy
@@ -406,23 +407,23 @@
             wavemin=wavemin, wavemax=wavemax)
 
     def __eq__(self, other):
 
         if self.wavemin is None and other.wavemin is None:
             wavemins_equal = True
         elif not all([self.wavemin, other.wavemin]):
-            # This means one is None and the other isn't
+            # This means one is None and the other isnt
             wavemins_equal = False
         else:
             wavemins_equal = np.allclose([self.wavemin], [other.wavemin], equal_nan=True)
 
         if self.wavemax is None and other.wavemax is None:
             wavemaxs_equal = True
         elif not all([self.wavemax, other.wavemax]):
-            # This means one is None and the other isn't
+            # This means one is None and the other isnt
             wavemaxs_equal = False
         else:
             wavemaxs_equal = np.allclose([self.wavemax], [other.wavemax], equal_nan=True)
 
         return (
             (self.id == other.id or self.id is None or other.id is None) and
             self.source == other.source and
```

### Comparing `sunpy-4.1.5/sunpy/database/tests/test_attrs.py` & `sunpy-4.1rc1/sunpy/database/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/tests/test_caching.py` & `sunpy-4.1rc1/sunpy/database/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/tests/test_commands.py` & `sunpy-4.1rc1/sunpy/database/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/tests/test_database.py` & `sunpy-4.1rc1/sunpy/database/tests/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -726,15 +726,14 @@
     assert not filled_database
     assert filled_database.session.query(JSONDump).all() == []
     assert filled_database.session.query(FitsHeaderEntry).all() == []
     assert filled_database.session.query(FitsKeyComment).all() == []
     assert filled_database.session.query(Tag).all() == []
     filled_database.undo()
     assert len(filled_database) == 10
-    assert len(filled_database.session.query(Tag).all()) == 2
     filled_database.redo()
     assert not filled_database
     assert filled_database.session.query(JSONDump).all() == []
     assert filled_database.session.query(FitsHeaderEntry).all() == []
     assert filled_database.session.query(FitsKeyComment).all() == []
     assert filled_database.session.query(Tag).all() == []
```

### Comparing `sunpy-4.1.5/sunpy/database/tests/test_table.txt` & `sunpy-4.1rc1/sunpy/database/tests/test_table.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/database/tests/test_tables.py` & `sunpy-4.1rc1/sunpy/database/tests/test_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         observation_time_end=datetime(2012, 1, 2, 0, 0),
         size=None,
         instrument='EVE',
         wavemin=0.1, wavemax=30.4)
     # 2 entries from goes
     assert entries[60] == DatabaseEntry(
         source='GOES', provider='NOAA', physobs='irradiance',
-        fileid='https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/goes15/'
+        fileid='https://satdat.ngdc.noaa.gov/sem/goes/data/science/xrs/goes15/'
                'gxrs-l2-irrad_science/2012/01/sci_gxrs-l2-irrad_g15_d20120101_v0-0-0.nc',
         observation_time_start=datetime(2012, 1, 1, 0, 0),
         observation_time_end=datetime(2012, 1, 1, 23, 59, 59, 999000),
         wavemin=np.nan, wavemax=np.nan,
         instrument='XRS')
     # 1 entry from noaa-indices
     assert entries[62] == DatabaseEntry(
@@ -185,19 +185,19 @@
         source='NAOJ', provider='NRO', physobs=None,
         fileid=("ftp://solar-pub.nao.ac.jp/"
                 "pub/nsro/norh/data/tcx/2012/01/tca120101"),
         observation_time_start=datetime(2012, 1, 1, 0, 0),
         observation_time_end=datetime(2012, 1, 1, 23, 59, 59, 999000),
         wavemin=17634850.470588233, wavemax=17634850.470588233,
         instrument='NORH')
-    # 2 entries from rhessi
-    assert 'hsi_obssumm_20120101' in entries[66].fileid
+    # 1 entry from rhessi
     assert entries[66] == DatabaseEntry(
         source="RHESSI", provider='NASA', physobs='summary_lightcurve',
-        fileid=entries[66].fileid,
+        fileid=("https://hesperia.gsfc.nasa.gov/"
+                "hessidata/metadata/catalog/hsi_obssumm_20120101_032.fits"),
         observation_time_start=datetime(2012, 1, 1, 0, 0),
         observation_time_end=datetime(2012, 1, 1, 23, 59, 59, 999000),
         wavemin=np.nan, wavemax=np.nan,
         instrument='RHESSI')
 
 
 @pytest.mark.remote_data
```

### Comparing `sunpy-4.1.5/sunpy/extern/README.rst` & `sunpy-4.1rc1/sunpy/extern/README.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/appdirs.py` & `sunpy-4.1rc1/sunpy/extern/appdirs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/appdirs_license.txt` & `sunpy-4.1rc1/sunpy/extern/appdirs_license.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/distro.py` & `sunpy-4.1rc1/sunpy/extern/distro.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/distro_license.rst` & `sunpy-4.1rc1/sunpy/extern/distro_license.rst`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/inflect.py` & `sunpy-4.1rc1/sunpy/extern/inflect.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/inflect_license.txt` & `sunpy-4.1rc1/sunpy/extern/inflect_license.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/parse.py` & `sunpy-4.1rc1/sunpy/extern/parse.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/extern/parse_license.txt` & `sunpy-4.1rc1/sunpy/extern/parse_license.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/image/resample.py` & `sunpy-4.1rc1/sunpy/image/resample.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     Returns a new `numpy.ndarray` that has been resampled up or down.
 
     Arbitrary resampling of source array to new dimension sizes.
     Currently only supports maintaining the same number of dimensions.
     To use 1-D arrays, first promote them to shape (x,1).
 
-    Uses the same parameters and creates the same coordinate lookup points
+    Uses the same parameters and creates the same co-ordinate lookup points
     as IDL's ``congrid`` routine (which apparently originally came from a
     VAX/VMS routine of the same name.)
 
     Parameters
     ----------
     orig : `numpy.ndarray`
         Original input array.
```

### Comparing `sunpy-4.1.5/sunpy/image/tests/test_resample.py` & `sunpy-4.1rc1/sunpy/image/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/image/tests/test_transform.py` & `sunpy-4.1rc1/sunpy/image/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/image/transform.py` & `sunpy-4.1rc1/sunpy/image/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ----------
     image : `numpy.ndarray`
         2D image to be rotated.
     rmatrix : `numpy.ndarray` that is 2x2
         Linear transformation rotation matrix.
     order : `int` 0-5, optional
         Interpolation order to be used, defaults to 3.  The precise meaning depends
-        on the rotation method specified by ``method``.
+        on the rotation method specifed by ``method``.
     scale : `float`
         A scale factor for the image with the default being no scaling.
     image_center : tuple, optional
         The point in the image to rotate around (axis of rotation).
         Defaults to the center of the array.
     recenter : `bool` or array-like, optional
         Move the axis of rotation to the center of the array or recenter coords.
```

### Comparing `sunpy-4.1.5/sunpy/io/_fits.py` & `sunpy-4.1rc1/sunpy/io/_fits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module provides a FITS file reader.
 
 .. warning::
 
    ``sunpy.io.fits`` is deprecated, and will be removed in sunpy 4.1. This is
-   because it was designed for internal use only. We instead recommend users
+   because it was designed for interal use only. We instead recommend users
    use the `astropy.io.fits` module, which provides more generic functionality
    to read FITS files.
 
 
 Notes
 -----
```

### Comparing `sunpy-4.1.5/sunpy/io/ana.py` & `sunpy-4.1rc1/sunpy/io/ana.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/cdf.py` & `sunpy-4.1rc1/sunpy/io/cdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/file_tools.py` & `sunpy-4.1rc1/sunpy/io/file_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module provides a generic file reader.
 """
+import os
 import re
-import gzip
 import pathlib
 
 try:
     from . import _fits as fits
 except ImportError:
     fits = None
 
@@ -210,19 +210,22 @@
         fp.seek(0)
         first_8bytes = fp.read(8)
         # first 4 bytes of CDF
         fp.seek(0)
         cdf_magic_number = fp.read(4).hex()
 
     # FITS
-    # Checks for gzip signature.
-    # If found, decompresses first few bytes and checks for FITS
-    if first80[:3] == b"\x1f\x8b\x08":
-        with gzip.open(filepath, 'rb') as fp:
-            first80 = fp.read(80)
+    # Check the extensions to see if it is a gzipped FITS file
+    filepath_rest_ext1, ext1 = os.path.splitext(filepath)
+    _, ext2 = os.path.splitext(filepath_rest_ext1)
+
+    gzip_extensions = [".gz"]
+    fits_extensions = [".fts", ".fit", ".fits"]
+    if (ext1 in gzip_extensions and ext2 in fits_extensions):
+        return 'fits'
 
     # Check for "KEY_WORD  =" at beginning of file
     match = re.match(br"[A-Z0-9_]{0,8} *=", first80)
     if match is not None:
         return 'fits'
 
     # JPEG 2000
```

### Comparing `sunpy-4.1.5/sunpy/io/jp2.py` & `sunpy-4.1rc1/sunpy/io/jp2.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/setup_package.py` & `sunpy-4.1rc1/sunpy/io/setup_package.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/converters/frames.py` & `sunpy-4.1rc1/sunpy/io/special/asdf/converters/frames.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/converters/generic_map.py` & `sunpy-4.1rc1/sunpy/io/special/asdf/converters/generic_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/entry_points.py` & `sunpy-4.1rc1/sunpy/io/special/asdf/entry_points.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml` & `sunpy-4.1rc1/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/tests/helpers.py` & `sunpy-4.1rc1/sunpy/io/special/asdf/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/tests/hgc_100.asdf` & `sunpy-4.1rc1/sunpy/io/special/asdf/tests/hgc_100.asdf`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/tests/test_coordinate_frames.py` & `sunpy-4.1rc1/sunpy/io/special/asdf/tests/test_coordinate_frames.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/asdf/tests/test_genericmap.py` & `sunpy-4.1rc1/sunpy/io/special/asdf/tests/test_genericmap.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/genx.py` & `sunpy-4.1rc1/sunpy/io/special/genx.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/special/srs.py` & `sunpy-4.1rc1/sunpy/io/special/srs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     header, section_lines = split_lines(file_lines)
 
     return make_table(header, section_lines)
 
 
 def make_table(header, section_lines):
     """
-    From the separated section lines and the header, clean up the data and
+    From the seperated section lines and the header, clean up the data and
     convert to a `~astropy.table.QTable`.
     """
     meta_data = get_meta_data(header)
 
     tables = []
     for i, lines in enumerate(section_lines):
         if lines:
```

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/_pyana.c` & `sunpy-4.1rc1/sunpy/io/src/ana/_pyana.c`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/anacompress.c` & `sunpy-4.1rc1/sunpy/io/src/ana/anacompress.c`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/anacompress.h` & `sunpy-4.1rc1/sunpy/io/src/ana/anacompress.h`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/anadecompress.c` & `sunpy-4.1rc1/sunpy/io/src/ana/anadecompress.c`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/anadecompress.h` & `sunpy-4.1rc1/sunpy/io/src/ana/anadecompress.h`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/anarw.c` & `sunpy-4.1rc1/sunpy/io/src/ana/anarw.c`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/anarw.h` & `sunpy-4.1rc1/sunpy/io/src/ana/anarw.h`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/src/ana/types.h` & `sunpy-4.1rc1/sunpy/io/src/ana/types.h`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/tests/generate_genx.pro` & `sunpy-4.1rc1/sunpy/io/tests/generate_genx.pro`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/tests/test_ana.py` & `sunpy-4.1rc1/sunpy/io/tests/test_ana.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pytest
 
 from sunpy.io import ana
 from sunpy.tests.helpers import skip_ana
 
 img_size = (456, 345)
-img_src = np.arange(np.prod(img_size))
+img_src = np.arange(np.product(img_size))
 img_src.shape = img_size
 img_i8 = img_src*2**8/img_src.max()
 img_i8 = img_i8.astype(np.int8)
 img_i16 = img_src*2**16/img_src.max()
 img_i16 = img_i16.astype(np.int16)
 img_f32 = img_src*1.0/img_src.max()
 img_f32 = img_f32.astype(np.float32)
```

### Comparing `sunpy-4.1.5/sunpy/io/tests/test_cdf.py` & `sunpy-4.1rc1/sunpy/io/tests/test_cdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/tests/test_filetools.py` & `sunpy-4.1rc1/sunpy/io/tests/test_filetools.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,17 +45,16 @@
     assert all([isinstance(p[0], np.ndarray) for p in pairs])
     assert all([isinstance(p[1],
                            sunpy.io.header.FileHeader) for p in pairs])
 
 
 def test_read_file_fits_gzip():
     # Test read gzipped fits file
-    gzip_fits_files = ["gzip_test.fts.gz", "gzip_test.fits.gz", "gzip_test.fit.gz", "gzip_fits_test.file"]
-    for filename in gzip_fits_files:
-        pair = sunpy.io.read_file(get_test_filepath(filename))
+    for fits_extension in [".fts", ".fit", ".fits"]:
+        pair = sunpy.io.read_file(get_test_filepath(f"gzip_test{fits_extension}.gz"))
         assert isinstance(pair, list)
         assert len(pair) == 1
         assert len(pair[0]) == 2
         assert isinstance(pair[0][0], np.ndarray)
         assert isinstance(pair[0][1], sunpy.io.header.FileHeader)
         assert np.all(pair[0][0] == np.tile(np.arange(32), (32, 1)).transpose())
```

### Comparing `sunpy-4.1.5/sunpy/io/tests/test_fits.py` & `sunpy-4.1rc1/sunpy/io/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/tests/test_genx.py` & `sunpy-4.1rc1/sunpy/io/tests/test_genx.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/io/tests/test_jp2.py` & `sunpy-4.1rc1/sunpy/io/tests/test_jp2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 TEST_AIA_IMAGE = get_test_filepath('aia_171_level1.fits')
 
 
 @skip_glymur
 def test_read():
     data, header = jp2.read(AIA_193_JP2)[0]
     assert isinstance(data, np.ndarray)
-    assert data.shape == (410, 410)
+    assert data.shape == (4096, 4096)
     assert isinstance(header, FileHeader)
 
 
 @skip_glymur
 def test_read_header():
     header = jp2.get_header(AIA_193_JP2)[0]
     assert isinstance(header, FileHeader)
```

### Comparing `sunpy-4.1.5/sunpy/io/tests/test_srs.py` & `sunpy-4.1rc1/sunpy/io/tests/test_srs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/compositemap.py` & `sunpy-4.1rc1/sunpy/map/compositemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         Notes
         -----
         Images are plotted using either `~matplotlib.axes.Axes.imshow` or
         `~matplotlib.axes.Axes.pcolormesh`, and contours are plotted using
         `~matplotlib.axes.Axes.contour`.
         The Matplotlib arguments accepted by the plotting method are passed to it.
-        (For compatibility reasons, we enforce a more restrictive set of
+        (For compatability reasons, we enforce a more restrictive set of
         accepted `~matplotlib.axes.Axes.pcolormesh` arguments.)
         If any Matplotlib arguments are not used by any plotting method,
         a ``TypeError`` will be raised.
         The ``sunpy.map.compositemap`` module includes variables which list the
         full set of arguments passed to each plotting method. These are:
 
         >>> import sunpy.map.compositemap
```

### Comparing `sunpy-4.1.5/sunpy/map/header_helper.py` & `sunpy-4.1rc1/sunpy/map/header_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 def _set_rotation_params(meta_wcs, rotation_angle, rotation_matrix):
     if rotation_angle is not None and rotation_matrix is not None:
         raise ValueError("Can not specify both rotation angle and rotation matrix.")
     if rotation_angle is None and rotation_matrix is None:
         rotation_angle = 0 * u.deg
 
     if rotation_angle is not None:
-        lam = meta_wcs['cdelt2'] / meta_wcs['cdelt1']
+        lam = meta_wcs['cdelt1'] / meta_wcs['cdelt2']
         p = np.deg2rad(rotation_angle)
 
         rotation_matrix = np.array([[np.cos(p), -1 * lam * np.sin(p)],
                                     [1/lam * np.sin(p), np.cos(p)]])
 
     if rotation_matrix is not None:
         (meta_wcs['PC1_1'], meta_wcs['PC1_2'],
@@ -223,15 +223,15 @@
     Returns
     -------
     `dict`
         Containing the WCS meta information
             * ctype1, ctype2
             * cunit1, cunit2
             * date_obs
-            * observer auxiliary information, if set on `coordinate`
+            * observer auxillary information, if set on `coordinate`
     """
 
     coord_meta = {}
 
     skycoord_wcs = astropy.wcs.utils.celestial_frame_to_wcs(coordinate, projection_code)
 
     cunit1, cunit2 = skycoord_wcs.wcs.cunit
```

### Comparing `sunpy-4.1.5/sunpy/map/map_factory.py` & `sunpy-4.1rc1/sunpy/map/map_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         # call a fits file or a jpeg2k file, etc
         # NOTE: use os.fspath so that fname can be either a str or pathlib.Path
         # This can be removed once read_file supports pathlib.Path
         log.debug(f'Reading {fname}')
         try:
             pairs = read_file(os.fspath(fname), **kwargs)
         except Exception as e:
-            msg = f"Failed to read {fname}"
+            msg = f"Failed to read {fname}."
             raise IOError(msg) from e
 
         new_pairs = []
         for pair in pairs:
             filedata, filemeta = pair
             assert isinstance(filemeta, FileHeader)
             # This tests that the data is more than 1D
```

### Comparing `sunpy-4.1.5/sunpy/map/mapbase.py` & `sunpy-4.1rc1/sunpy/map/mapbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from dask.array import Array as DaskArray
     DASK_INSTALLED = True
 except ImportError:
     DASK_INSTALLED = False
 
 import astropy.units as u
 import astropy.wcs
-from astropy.coordinates import BaseCoordinateFrame, Longitude, SkyCoord, UnitSphericalRepresentation
+from astropy.coordinates import Longitude, SkyCoord, UnitSphericalRepresentation
 from astropy.nddata import NDData
 from astropy.utils.metadata import MetaData
 from astropy.visualization import AsymmetricPercentileInterval, HistEqStretch, ImageNormalize
 from astropy.visualization.wcsaxes import Quadrangle, WCSAxes
 
 # The next two are not used but are called to register functions with external modules
 import sunpy.coordinates
@@ -64,15 +64,15 @@
 _META_FIX_URL = 'https://docs.sunpy.org/en/stable/code_ref/map.html#fixing-map-metadata'
 
 # Manually specify the ``.meta`` docstring. This is assigned to the .meta
 # class attribute in GenericMap.__init__()
 _meta_doc = """
 The map metadata.
 
-This is used to interpret the map data. It may
+This is used to intepret the map data. It may
 have been modified from the original metadata by sunpy. See the
 `~sunpy.util.MetaDict.added_items`, `~sunpy.util.MetaDict.removed_items`
 and `~sunpy.util.MetaDict.modified_items` properties of MetaDict
 to query how the metadata has been modified.
 """
 
 # The notes live here so we can reuse it in the source maps
@@ -99,15 +99,15 @@
     If a header has CD_ij values but no PC_ij values, CDELT values are required
     for this class to construct the WCS.
     If a file with more than two dimensions is feed into the class,
     only the first two dimensions (NAXIS1, NAXIS2) will be loaded and the
     rest will be discarded.
 """
 
-__all__ = ['GenericMap', 'MapMetaValidationError', 'PixelPair']
+__all__ = ['GenericMap', 'MapMetaValidationError']
 
 
 class MapMetaValidationError(AttributeError):
     pass
 
 
 class GenericMap(NDData):
@@ -575,17 +575,15 @@
         return self._new_instance_from_op(new_data)
 
     @property
     def _meta_hash(self):
         return self.meta.item_hash()
 
     def _set_symmetric_vmin_vmax(self):
-        """
-        Set symmetric vmin and vmax about zero
-        """
+        # Set symmetric vmin/vmax about zero
         threshold = np.nanmax(abs(self.data))
         self.plot_settings['norm'].vmin = -threshold
         self.plot_settings['norm'].vmax = threshold
 
     @property
     @cached_property_based_on('_meta_hash')
     def wcs(self):
@@ -594,15 +592,15 @@
         """
         w2 = astropy.wcs.WCS(naxis=2)
 
         # Add one to go from zero-based to one-based indexing
         w2.wcs.crpix = u.Quantity(self.reference_pixel) + 1 * u.pix
         # Make these a quantity array to prevent the numpy setting element of
         # array with sequence error.
-        # Explicitly call ``.to()`` to check that scale is in the correct units
+        # Explicityly call ``.to()`` to check that scale is in the correct units
         w2.wcs.cdelt = u.Quantity([self.scale[0].to(self.spatial_units[0] / u.pix),
                                    self.scale[1].to(self.spatial_units[1] / u.pix)])
         w2.wcs.crval = u.Quantity([self._reference_longitude, self._reference_latitude])
         w2.wcs.ctype = self.coordinate_system
         w2.wcs.pc = self.rotation_matrix
         w2.wcs.set_pv(self._pv_values)
         # FITS standard doesn't allow both PC_ij *and* CROTA keywords
@@ -833,15 +831,15 @@
 
     @property
     def date_average(self):
         """
         Average time of the image acquisition.
 
         Taken from the DATE-AVG FITS keyword if present, otherwise halfway
-        between `date_start` and `date_end` if both pieces of metadata are
+        between `date_start` and `date_end` if both peices of metadata are
         present.
         """
         avg = self._get_date('date-avg')
         if avg is None:
             start, end = self.date_start, self.date_end
             if start is not None and end is not None:
                 avg = start + (end - start) / 2
@@ -1269,30 +1267,18 @@
                          (self.meta.get('crpix2', (naxis2 + 1) / 2.) - 1) * u.pixel)
 
     @property
     def scale(self):
         """
         Image scale along the x and y axes in units/pixel
         (i.e. cdelt1, cdelt2).
-
-        If the CDij matrix is defined but no CDELTi values are explicitly defined,
-        effective CDELTi values are constructed from the CDij matrix.  The effective
-        CDELTi values are chosen so that each row of the PCij matrix has unity norm.
-        This choice is optimal if the PCij matrix is a pure rotation matrix, but may not
-        be as optimal if the PCij matrix includes any skew.
-        """
-        if 'cd1_1' in self.meta and 'cdelt1' not in self.meta and 'cdelt2' not in self.meta:
-            cdelt1 = np.sqrt(self.meta['cd1_1']**2 + self.meta['cd1_2']**2)
-            cdelt2 = np.sqrt(self.meta['cd2_1']**2 + self.meta['cd2_2']**2)
-        else:
-            cdelt1 = self.meta.get('cdelt1', 1.)
-            cdelt2 = self.meta.get('cdelt2', 1.)
-
-        return SpatialPair(cdelt1 * self.spatial_units[0] / u.pixel,
-                           cdelt2 * self.spatial_units[1] / u.pixel)
+        """
+        # TODO: Fix this if only CDi_j matrix is provided
+        return SpatialPair(self.meta.get('cdelt1', 1.) * self.spatial_units[0] / u.pixel,
+                           self.meta.get('cdelt2', 1.) * self.spatial_units[1] / u.pixel)
 
     @property
     def spatial_units(self):
         """
         Image coordinate units along the x and y axes (i.e. cunit1, cunit2).
         """
         units = self.meta.get('cunit1', None), self.meta.get('cunit2', None)
@@ -1301,15 +1287,15 @@
 
     @property
     def rotation_matrix(self):
         r"""
         Matrix describing the transformation needed to align the reference
         pixel with the coordinate axes.
 
-        The order or precedence of FITS keywords which this is taken from is:
+        The order or precendence of FITS keywords which this is taken from is:
         - PC\*_\*
         - CD\*_\*
         - CROTA\*
 
         Notes
         -----
         In many cases this is a simple rotation matrix, hence the property name.
@@ -1322,16 +1308,15 @@
 
         elif 'CD1_1' in self.meta:
             cd = np.array([[self.meta['CD1_1'], self.meta['CD1_2']],
                            [self.meta['CD2_1'], self.meta['CD2_2']]])
 
             cdelt = u.Quantity(self.scale).value
 
-            # Divide each row by each CDELT
-            return cd / np.expand_dims(cdelt, axis=1)
+            return cd / cdelt
         else:
             return self._rotation_matrix_from_crota()
 
     @staticmethod
     def _pc_matrix(lam, angle):
         """
         Returns PC matrix from the scale ration (lam) and rotation
@@ -1508,15 +1493,15 @@
 # #### Image processing routines #### #
 
     @u.quantity_input
     def resample(self, dimensions: u.pixel, method='linear'):
         """
         Resample to new dimension sizes.
 
-        Uses the same parameters and creates the same coordinate lookup points
+        Uses the same parameters and creates the same co-ordinate lookup points
         as IDL''s congrid routine, which apparently originally came from a
         VAX/VMS routine of the same name.
 
         Parameters
         ----------
         dimensions : `~astropy.units.Quantity`
             Output pixel dimensions. The first argument corresponds to the 'x'
@@ -1553,22 +1538,28 @@
         scale_factor_x = float(self.dimensions[0] / dimensions[0])
         scale_factor_y = float(self.dimensions[1] / dimensions[1])
 
         # Update image scale and number of pixels
         new_meta = self.meta.copy()
 
         # Update metadata
-        for key in {'cdelt1', 'cd1_1', 'cd2_1'} & self.meta.keys():
-            new_meta[key] *= scale_factor_x
-        for key in {'cdelt2', 'cd1_2', 'cd2_2'} & self.meta.keys():
-            new_meta[key] *= scale_factor_y
         if 'pc1_1' in self.meta:
-            new_meta['pc1_2'] *= scale_factor_y / scale_factor_x
-            new_meta['pc2_1'] *= scale_factor_x / scale_factor_y
-
+            new_meta['pc1_1'] *= scale_factor_x
+            new_meta['pc2_1'] *= scale_factor_x
+            new_meta['pc1_2'] *= scale_factor_y
+            new_meta['pc2_2'] *= scale_factor_y
+        if 'cd1_1' in self.meta:
+            new_meta['cd1_1'] *= scale_factor_x
+            new_meta['cd2_1'] *= scale_factor_x
+            new_meta['cd1_2'] *= scale_factor_y
+            new_meta['cd2_2'] *= scale_factor_y
+        if 'cd1_1' not in self.meta and 'pc1_1' not in self.meta:
+            # Using the CROTA2 and CDELT formalism
+            new_meta['cdelt1'] *= scale_factor_x
+            new_meta['cdelt2'] *= scale_factor_y
         new_meta['crpix1'] = (self.reference_pixel.x.to_value(u.pix) + 0.5) / scale_factor_x + 0.5
         new_meta['crpix2'] = (self.reference_pixel.y.to_value(u.pix) + 0.5) / scale_factor_y + 0.5
         new_meta['naxis1'] = new_data.shape[1]
         new_meta['naxis2'] = new_data.shape[0]
 
         # Create new map instance
         new_map = self._new_instance(new_data, new_meta, self.plot_settings)
@@ -1974,26 +1965,21 @@
             top_right = u.Quantity([bottom_left[0] + width, bottom_left[1] + height])
 
         top_left = u.Quantity([top_right[0], bottom_left[1]])
         bottom_right = u.Quantity([bottom_left[0], top_right[1]])
         return bottom_left, top_left, top_right, bottom_right
 
     @_parse_submap_input.register(SkyCoord)
-    @_parse_submap_input.register(BaseCoordinateFrame)
     def _parse_submap_coord_input(self, bottom_left, top_right, width, height):
         # Use helper function to get top_right as a SkyCoord
         bottom_left, top_right = get_rectangle_coordinates(bottom_left,
                                                            top_right=top_right,
                                                            width=width,
                                                            height=height)
-
-        if isinstance(bottom_left, SkyCoord):
-            frame = bottom_left.frame
-
-        frame = bottom_left
+        frame = bottom_left.frame
         left_lon, bottom_lat = self._get_lon_lat(bottom_left)
         right_lon, top_lat = self._get_lon_lat(top_right)
         corners = SkyCoord([left_lon, left_lon, right_lon, right_lon],
                            [bottom_lat, top_lat, top_lat, bottom_lat],
                            frame=frame)
 
         return tuple(u.Quantity(self.wcs.world_to_pixel(corners), u.pix).T)
@@ -2062,28 +2048,33 @@
 
         # Update image scale and number of pixels
 
         # create copy of new meta data
         new_meta = self.meta.copy()
 
         # Update metadata
-        for key in {'cdelt1', 'cd1_1', 'cd2_1'} & self.meta.keys():
-            new_meta[key] *= dimensions[0]
-        for key in {'cdelt2', 'cd1_2', 'cd2_2'} & self.meta.keys():
-            new_meta[key] *= dimensions[1]
         if 'pc1_1' in self.meta:
-            new_meta['pc1_2'] *= dimensions[1] / dimensions[0]
-            new_meta['pc2_1'] *= dimensions[0] / dimensions[1]
+            new_meta['pc1_1'] *= dimensions[0]
+            new_meta['pc2_1'] *= dimensions[0]
+            new_meta['pc1_2'] *= dimensions[1]
+            new_meta['pc2_2'] *= dimensions[1]
+        if 'cd1_1' in self.meta:
+            new_meta['cd1_1'] *= dimensions[0]
+            new_meta['cd2_1'] *= dimensions[0]
+            new_meta['cd1_2'] *= dimensions[1]
+            new_meta['cd2_2'] *= dimensions[1]
+        if 'cd1_1' not in self.meta and 'pc1_1' not in self.meta:
+            # Using the CROTA2 and CDELT formalism
+            new_meta['cdelt1'] *= dimensions[0]
+            new_meta['cdelt2'] *= dimensions[1]
 
         new_meta['crpix1'] = ((self.reference_pixel.x.to_value(u.pix) +
                                0.5 - offset[0]) / dimensions[0]) + 0.5
         new_meta['crpix2'] = ((self.reference_pixel.y.to_value(u.pix) +
                                0.5 - offset[1]) / dimensions[1]) + 0.5
-        new_meta['naxis1'] = new_array.shape[1]
-        new_meta['naxis2'] = new_array.shape[0]
 
         # Create new map instance
         if self.mask is not None:
             new_data = np.ma.getdata(new_array)
             new_mask = np.ma.getmask(new_array)
         else:
             new_data = new_array
@@ -2262,15 +2253,15 @@
         else:
             bottom_left, top_right = get_rectangle_coordinates(
                 bottom_left, top_right=top_right, width=width, height=height)
 
             width = Longitude(top_right.spherical.lon - bottom_left.spherical.lon)
             height = top_right.spherical.lat - bottom_left.spherical.lat
             anchor = self._get_lon_lat(bottom_left)
-            transform = axes.get_transform(bottom_left.replicate_without_data())
+            transform = axes.get_transform(bottom_left.frame.replicate_without_data())
 
         kwergs = {
             "transform": transform,
             "edgecolor": "white",
             "fill": False,
         }
         kwergs.update(kwargs)
@@ -2546,17 +2537,15 @@
 
             # The quadrilaterals of pcolormesh can slightly overlap, which creates the appearance
             # of a grid pattern when alpha is not 1.  These settings minimize the overlap.
             if imshow_args.get('alpha', 1) != 1:
                 imshow_args.setdefault('antialiased', True)
                 imshow_args.setdefault('linewidth', 0)
 
-            ret = axes.pcolormesh(np.arange(data.shape[1] + 1) - 0.5,
-                                  np.arange(data.shape[0] + 1) - 0.5,
-                                  data, **imshow_args)
+            ret = axes.pcolormesh(data, **imshow_args)
         else:
             ret = axes.imshow(data, **imshow_args)
 
         wcsaxes_compat.default_wcs_grid(axes)
 
         # Set current axes/image if pyplot is being used (makes colorbar work)
         for i in plt.get_fignums():
```

### Comparing `sunpy-4.1.5/sunpy/map/mapsequence.py` & `sunpy-4.1rc1/sunpy/map/mapsequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         nmaps = len(self)
 
         # Output a warning about rendering time if there are more than 9 Maps
         if nmaps > 9:
             warn_user(f"Rendering the summary for a MapSequence of {nmaps} Maps "
                       "may take a while.")
 
-        # Assemble the individual HTML repr from each Map, all hidden initially
+        # Assemble the individual HTML repr from each Map, all hidden initally
         repr_list = [f"<div style='display: none' index={i}>{m._repr_html_()}</div>"
                      for i, m in enumerate(self.maps)]
 
         # Unhide the first Map
         repr_list_html = "\n".join(repr_list).replace('display: none', 'display: ', 1)
 
         # Return HTML with Javascript-powered buttons
```

### Comparing `sunpy-4.1.5/sunpy/map/maputils.py` & `sunpy-4.1rc1/sunpy/map/maputils.py`

 * *Files 9% similar despite different names*

```diff
@@ -397,15 +397,15 @@
         The input coordinate.
 
     Returns
     -------
     bool
         `True` if ``coordinates`` falls within the bounds of ``smap``.
         This includes the edges of the map. If multiple coordinates are input,
-        returns a boolean array.
+        returns a boolean arrary.
     """
     # Dimensions of smap
     ys, xs = smap.wcs.array_shape
     # Converting coordinates to pixels
     xc, yc = smap.wcs.world_to_pixel(coordinates)
     return ((xc >= -0.5) &
             (xc <= xs - 0.5) &
@@ -450,46 +450,33 @@
             err = err + dx
             y += sy
     return np.array(res)
 
 
 def extract_along_coord(smap, coord):
     """
-    Extract pixel values from a map along a path that approximates a coordinate path.
+    Return the value of the image array at every pixel the coordinate path intersects.
 
-    Each pair of consecutive coordinates in the provided coordinate array defines a
-    line segment in pixel space.  The approximate pixel path for each line segment is
-    determined by applying
-    `Bresenham's line algorithm <http://en.wikipedia.org/wiki/Bresenham%27s_line_algorithm>`_.
-    The resulting pixel path does not necessarily include every pixel that is
-    intersected by each line segment.
+    For a given coordinate ``coord``, find all the pixels that cross the coordinate
+    and extract the values of the image array in ``smap`` at these points. This is done by applying
+    `Bresenham's line algorithm <http://en.wikipedia.org/wiki/Bresenham%27s_line_algorithm>`_
+    between the consecutive coordinates, in pixel space, and then indexing the data
+    array of ``smap`` at those points.
 
     Parameters
     ----------
     smap : `~sunpy.map.GenericMap`
         The sunpy map.
     coord : `~astropy.coordinates.SkyCoord`
-        The coordinate array that defines the path for extraction.
+        Coordinate along which to extract intensity.
 
     Returns
     -------
-    pixel_values : `~astropy.units.Quantity`
-         The pixel values along a path that approximates the coordinate path.
-    pixel_coords : `~astropy.coordinates.SkyCoord`
-         The coordinates for the pixels from which the values were extracted.
-
-    Notes
-    -----
-    The provided coordinates are first rounded to the nearest corresponding pixel,
-    which means that the coordinates used for calculations may be shifted relative
-    to the provided coordinates by up to half a pixel.
-
-    Examples
-    --------
-    .. minigallery:: sunpy.map.extract_along_coord
+    values : `~astropy.units.Quantity`
+    value_coords : `~astropy.coordinates.SkyCoord`
     """
     if not len(coord.shape) or coord.shape[0] < 2:
         raise ValueError('At least two points are required for extracting intensity along a '
                          'line. To extract points at single coordinates, use '
                          'sunpy.map.maputils.sample_at_coords.')
     if not all(contains_coordinate(smap, coord)):
         raise ValueError('At least one coordinate is not within the bounds of the map.'
@@ -503,11 +490,11 @@
         # Pop the last one, unless this is the final entry because the first point
         # of the next section will be the same
         if i < (len(px) - 2):
             b = b[:-1]
         pix.append(b)
     pix = np.vstack(pix)
 
-    pixel_values = u.Quantity(smap.data[pix[:, 0], pix[:, 1]], smap.unit)
-    pixel_coords = smap.wcs.pixel_to_world(pix[:, 1], pix[:, 0])
+    intensity = u.Quantity(smap.data[pix[:, 0], pix[:, 1]], smap.unit)
+    coord_new = smap.wcs.pixel_to_world(pix[:, 1], pix[:, 0])
 
-    return pixel_values, pixel_coords
+    return intensity, coord_new
```

### Comparing `sunpy-4.1.5/sunpy/map/sources/__init__.py` & `sunpy-4.1rc1/sunpy/map/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/hinode.py` & `sunpy-4.1rc1/sunpy/map/sources/hinode.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,27 +94,14 @@
     @property
     def processing_level(self):
         lvl = self.meta.get('DATA_LEV', None)
         if lvl is None:
             return
         return int(lvl)
 
-    @property
-    def unit(self):
-        # XRT data values are in DN and are converted into DN/s if the data has been normalized.
-        # A tag starting with "XRT_RENORMALIZE" is added to the HISTORY tag in that case.
-        # See Table 1.1 and Section 2.11 of the XRT Analysis Guide.
-        unit = super().unit
-        if not unit:
-            unit = u.ct
-            history = self.meta.get('HISTORY', '')
-            if "xrt_renormalize" in history.lower():
-                unit = u.ct / u.second
-        return unit
-
     @classmethod
     def is_datasource_for(cls, data, header, **kwargs):
         """Determines if header corresponds to an XRT image"""
         return header.get('instrume') == 'XRT'
 
 
 class SOTMap(GenericMap):
@@ -151,15 +138,15 @@
                         'FG shutterless I and V with 0.2s intervals',
                         'FG shutterless Stokes', 'SP IQUV 4D array']
 
     def __init__(self, data, header, **kwargs):
         super().__init__(data, header, **kwargs)
         self._nickname = self.detector
 
-        # TODO (add other options, Now all treated as intensity. This follows
+        # TODO (add other options, Now all threated as intensity. This follows
         # Hinode SDC archive) StokesQUV -> grey, Velocity -> EIS, Width -> EIS,
         # Mag Field Azi -> IDL 5 (STD gamma II)
         # 'WB' -> red
         # 'NB'(0 = red); (>0 = gray), # nb has 1 stokes I, the rest quv
         # 'SP' (<=1 = red); (>1 = gray) #sp has 2 stokes I, the rest quv
         color = {'SOT/WB': 'intensity',
                  'SOT/NB': 'intensity',  # For the 1st dimension
```

### Comparing `sunpy-4.1.5/sunpy/map/sources/iris.py` & `sunpy-4.1rc1/sunpy/map/sources/iris.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/mlso.py` & `sunpy-4.1rc1/sunpy/map/sources/mlso.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/proba2.py` & `sunpy-4.1rc1/sunpy/map/sources/proba2.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/psp.py` & `sunpy-4.1rc1/sunpy/map/sources/psp.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/rhessi.py` & `sunpy-4.1rc1/sunpy/map/sources/rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/sdo.py` & `sunpy-4.1rc1/sunpy/map/sources/sdo.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,19 +105,16 @@
     * `Instrument Page <http://hmi.stanford.edu>`_
     * `Analysis Guide <http://hmi.stanford.edu/doc/magnetic/guide.pdf>`_
     """
 
     def __init__(self, data, header, **kwargs):
         super().__init__(data, header, **kwargs)
         if self.unit is not None and self.unit.is_equivalent(u.T):
-            # Avoid JP2K images not having a norm due to UNIT8 data
-            # This means they are not scaled correctly.
-            if self.plot_settings.get('norm') is not None:
-                # Magnetic field maps, not intensity maps
-                self._set_symmetric_vmin_vmax()
+            # Magnetic field maps, not intensity maps
+            self._set_symmetric_vmin_vmax()
         self._nickname = self.detector
 
     @property
     def measurement(self):
         """
         Returns the measurement type.
         """
```

### Comparing `sunpy-4.1.5/sunpy/map/sources/soho.py` & `sunpy-4.1rc1/sunpy/map/sources/soho.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,30 +39,25 @@
 
         self._nickname = self.detector
         self.plot_settings['cmap'] = self._get_cmap_name()
         self.plot_settings['norm'] = ImageNormalize(
             stretch=source_stretch(self.meta, PowerStretch(0.5)), clip=False)
 
     @property
-    def date(self):
-        # Old EIT data has date-obs in format of dd-JAN-yy so we use date_obs where available
-        return self._get_date('date_obs') or super().date
-
-    @property
     def spatial_units(self):
         """
         If not present in CUNIT{1,2} keywords, defaults to arcsec.
         """
         return SpatialPair(u.Unit(self.meta.get('cunit1', 'arcsec')),
                            u.Unit(self.meta.get('cunit2', 'arcsec')))
 
     @property
     def waveunit(self):
         """
-        If WAVEUNIT FITS keyword isn't present, defaults to Angstrom.
+        If WAVEUNIT FITS keyword isn't present, deafults to Angstrom.
         """
         unit = self.meta.get("waveunit", "Angstrom") or "Angstrom"
         return u.Unit(unit)
 
     @property
     def detector(self):
         return "EIT"
@@ -92,15 +87,15 @@
     SOHO LASCO Image Map
 
     The Large Angle and Spectrometric COronagraph (LASCO) is a set of three
     Lyot-type coronagraphs (C1, C2, and C3) that image the solar corona from
     1.1 to 32 solar radii.
 
     The C1 images rom 1.1 to 3 solar radii. The C2 telescope images the corona
-    from 2 to 6 solar radii, overlapping the outer field-of-view of C1 from 2 to
+    from 2 to 6 solar radii, overlaping the outer field-of-view of C1 from 2 to
     3 solar radii. The C3 telescope extends the field-of-view to 32 solar radii.
 
     SOHO was launched on 2 December 2 1995 into a sun-synchronous orbit.
 
     References
     ----------
     * `SOHO Mission Page <https://sohowww.nascom.nasa.gov/>`_
@@ -132,15 +127,15 @@
             return np.identity(2)
         else:
             return super().rotation_matrix
 
     @property
     def date(self):
         date = self.meta.get('date-obs', self.meta.get('date_obs'))
-        # In case someone fixes the header
+        # Incase someone fixes the header
         if 'T' in date:
             return parse_time(date)
 
         time = self.meta.get('time-obs', self.meta.get('time_obs'))
         return parse_time(f"{date}T{time}")
 
     @property
@@ -189,15 +184,15 @@
         if self.unit is not None and self.unit.is_equivalent(u.T):
             # Magnetic field maps, not intensity maps
             self._set_symmetric_vmin_vmax()
 
     @property
     def _date_obs(self):
         if 'T' in self.meta['date-obs']:
-            # Helioviewer MDI files have the full date in DATE_OBS, but we still
+            # Helioviewer MDI files have the full date in DATE_OBS, but we stil
             # want to let normal FITS files use DATE-OBS
             return parse_time(self.meta['date-obs'])
         else:
             return parse_time(self.meta['date_obs'])
 
     @property
     def unit(self):
```

### Comparing `sunpy-4.1.5/sunpy/map/sources/solo.py` & `sunpy-4.1rc1/sunpy/map/sources/solo.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/source_type.py` & `sunpy-4.1rc1/sunpy/map/sources/source_type.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/stereo.py` & `sunpy-4.1rc1/sunpy/map/sources/stereo.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/suvi.py` & `sunpy-4.1rc1/sunpy/map/sources/suvi.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_aia_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_aia_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_cor_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_cor_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_eit_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_eit_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Test cases for SOHO EITMap subclass
 """
 import pytest
 
 import astropy.units as u
 
-from sunpy.data.test import get_dummy_map_from_header, get_test_data_filenames, get_test_filepath
+from sunpy.data.test import get_dummy_map_from_header, get_test_data_filenames
 from sunpy.map.sources.soho import EITMap
 
 header_list = [f for f in get_test_data_filenames() if 'efz' in f.name and '.header' in f.name]
 
 __author__ = "Pritish C. (VaticanCameos)"
 
 
@@ -50,12 +50,7 @@
     # Tests that the default normalizer has clipping disabled
     assert not eit_map.plot_settings['norm'].clip
 
 
 def test_wcs(eit_map):
     # Smoke test that WCS is valid and can transform from pixels to world coordinates
     eit_map.pixel_to_world(0*u.pix, 0*u.pix)
-
-
-def test_old_eit_date():
-    eit_map = get_dummy_map_from_header(get_test_filepath("seit_00171_fd_19961211_1900.header"))
-    assert eit_map.date.value == '1996-12-11T19:00:14.254'
```

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_eui_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_eui_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_euvi_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_euvi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_hi_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_hi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_hmi_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_hmi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_hmi_synoptic_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_hmi_synoptic_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_iris_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_iris_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_kcor_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_kcor_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_lasco_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_lasco_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_mdi_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_mdi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_rhessi_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_rhessi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_sot_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_sot_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_source_type.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_source_type.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_suvi_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_suvi_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 
 def test_norm_clip(suvi):
     # Tests that the default normalizer has clipping disabled
     assert not suvi.plot_settings['norm'].clip
 
 
 # SUVI provides observer coordinate information in an OBSGEO system, so this test
-# needs remote data to access the latest IERS table to do a coordinate transformation from
-# OBSGEO to heliographic Stonyhurst coordinates.
+# needs remote data to access the latest IERS table to do a coordiante transformation from
+# OBSGEO to heliographic Stonyhurst coordiantes.
 @pytest.mark.remote_data
 def test_wcs(suvi):
     # Smoke test that WCS is valid and can transform from pixels to world coordinates
     suvi.pixel_to_world(0*u.pix, 0*u.pix)
```

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_swap_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_swap_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_sxt_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_sxt_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_trace_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_trace_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_wispr_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_wispr_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/tests/test_xrt_source.py` & `sunpy-4.1rc1/sunpy/map/sources/tests/test_xrt_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,19 +34,14 @@
 
 
 def test_measurement(xrt_map):
     """Tests the measurement property of the XRTMap object."""
     assert xrt_map.measurement == 'Be thin-Open'
 
 
-def test_unit(xrt_map):
-    """Tests the unit property of the XRTMap object."""
-    assert xrt_map.unit == u.ct / u.second
-
-
 def test_level_number(xrt_map):
     assert xrt_map.processing_level == 1
 
 
 def test_heliographic_longitude(xrt_map):
     assert u.allclose(xrt_map.heliographic_longitude, 0 * u.deg)
```

### Comparing `sunpy-4.1.5/sunpy/map/sources/trace.py` & `sunpy-4.1rc1/sunpy/map/sources/trace.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/sources/yohkoh.py` & `sunpy-4.1rc1/sunpy/map/sources/yohkoh.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/tests/conftest.py` & `sunpy-4.1rc1/sunpy/map/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/tests/strategies.py` & `sunpy-4.1rc1/sunpy/map/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_compositemap.py` & `sunpy-4.1rc1/sunpy/map/tests/test_compositemap.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_header.py` & `sunpy-4.1rc1/sunpy/map/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_header_helper.py` & `sunpy-4.1rc1/sunpy/map/tests/test_header_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,41 +62,27 @@
 
 
 def test_metakeywords():
     meta = sunpy.map.meta_keywords()
     assert isinstance(meta, dict)
 
 
-def test_scale_conversion(map_data, hpc_coord):
-    # The header will have cunit1/2 of arcsec
-    header = make_fitswcs_header(map_data, hpc_coord, scale=[1, 2] * u.arcmin / u.pix)
-    assert header['cdelt1'] == 60
-    assert header['cdelt2'] == 120
-
-
-def test_default_rotation(map_data, hpc_coord):
+def test_deafult_rotation(map_data, hpc_coord):
     header = make_fitswcs_header(map_data, hpc_coord)
     wcs = WCS(header)
     np.testing.assert_allclose(wcs.wcs.pc, [[1, 0], [0, 1]], atol=1e-5)
 
 
 def test_rotation_angle(map_data, hpc_coord):
     header = make_fitswcs_header(map_data, hpc_coord,
                                  rotation_angle=90*u.deg)
     wcs = WCS(header)
     np.testing.assert_allclose(wcs.wcs.pc, [[0, -1], [1, 0]], atol=1e-5)
 
 
-def test_rotation_angle_rectangular_pixels(map_data, hpc_coord):
-    header = make_fitswcs_header(map_data, hpc_coord, scale=[2, 5] * u.arcsec / u.pix,
-                                 rotation_angle=45*u.deg)
-    wcs = WCS(header)
-    np.testing.assert_allclose(wcs.wcs.pc, np.sqrt(0.5) * np.array([[1, -2.5], [0.4, 1]]), atol=1e-5)
-
-
 def test_rotation_matrix(map_data, hpc_coord):
     header = make_fitswcs_header(map_data, hpc_coord,
                                  rotation_matrix=np.array([[1, 0], [0, 1]]))
     wcs = WCS(header)
     np.testing.assert_allclose(wcs.wcs.pc, [[1, 0], [0, 1]], atol=1e-5)
```

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_map_factory.py` & `sunpy-4.1rc1/sunpy/map/tests/test_map_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import os
 import pathlib
 import tempfile
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 
 from astropy.io import fits
 from astropy.wcs import WCS
 
 import sunpy
 import sunpy.map
 from sunpy.data.test import get_dummy_map_from_header, get_test_data_filenames, get_test_filepath, rootdir
-from sunpy.tests.helpers import figure_test, skip_glymur
+from sunpy.tests.helpers import skip_glymur
 from sunpy.util.exceptions import NoMapsInFileError, SunpyMetadataWarning, SunpyUserWarning
 
 a_list_of_many = [f for f in get_test_data_filenames() if 'efz' in f.name]
 
 AIA_171_IMAGE = get_test_filepath('aia_171_level1.fits')
 RHESSI_IMAGE = get_test_filepath('hsi_image_20101016_191218.fits')
 AIA_193_JP2 = get_test_filepath("2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2")
-HMI_LOS_JP2 = get_test_filepath("2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2")
 AIA_MAP = sunpy.map.Map(AIA_171_IMAGE)
 VALID_MAP_INPUTS = [
     (AIA_171_IMAGE, ),
     (pathlib.Path(AIA_171_IMAGE), ),
     (rootdir / "EIT", ),
     (os.fspath(rootdir / "EIT"), ),
     (rootdir / "EIT" / "*.fits", ),
@@ -177,15 +175,15 @@
     with pytest.raises(ValueError, match=nonexist_dir):
         sunpy.map.Map(os.fspath(directory))
 
     with pytest.raises(ValueError, match='Invalid input: 78'):
         # Check a random unsupported type (int) fails
         sunpy.map.Map(78)
 
-    # If one file failed to load, make sure it's raised as an exception.
+    # If one file failed to load, make sure it's raised as an expection.
     p = tmpdir.mkdir("sub").join("hello.fits")
     p.write("content")
     files = [AIA_171_IMAGE, p.strpath]
     with pytest.raises(OSError, match=(fr"Failed to read *")):
         sunpy.map.Map(files)
 
 
@@ -238,16 +236,16 @@
 
 
 @pytest.mark.remote_data
 def test_map_list_urls_cache():
     """
     Test for https://github.com/sunpy/sunpy/issues/4006
     """
-    urls = ['https://github.com/sunpy/data/raw/main/sunpy/v1/AIA20110607_063305_0094_lowres.fits',
-            'https://github.com/sunpy/data/raw/main/sunpy/v1/AIA20110607_063305_0094_lowres.fits']
+    urls = ['http://jsoc.stanford.edu/SUM80/D136597189/S00000/image_lev1.fits',
+            'http://jsoc.stanford.edu/SUM79/D136597240/S00000/image_lev1.fits']
     sunpy.map.Map(urls)
 
 
 @pytest.mark.filterwarnings('ignore:File may have been truncated')
 @pytest.mark.parametrize('file, mapcls', [
     ["EIT_header/efz20040301.000010_s.header", sunpy.map.sources.EITMap],
     ["lasco_c2_25299383_s.header", sunpy.map.sources.LASCOMap],
@@ -281,36 +279,25 @@
         sunpy.map.Map(tmp_fpath)
 
     with pytest.warns(SunpyUserWarning, match='One of the arguments failed to parse'):
         sunpy.map.Map([tmp_fpath, AIA_171_IMAGE], silence_errors=True)
 
 
 @skip_glymur
-def test_map_jp2_AIA():
+def test_map_jp2():
     jp2_map = sunpy.map.Map(AIA_193_JP2, memmap=False)
     assert isinstance(jp2_map, sunpy.map.GenericMap)
     # The base of an array that owns its memory is None
     # For some reason JP2 doesn't own its own memory but are not type of memmaps.
     assert jp2_map.data.base is not None
     jp2_map = sunpy.map.Map(AIA_193_JP2, memmap=True)
     assert isinstance(jp2_map, sunpy.map.GenericMap)
     assert jp2_map.data.base is not None
 
 
-@skip_glymur
-@figure_test
-def test_map_jp2_HMI():
-    # We failed to read the HMI JP2 file with map before
-    # See https://github.com/sunpy/sunpy/issues/6709
-    jp2_map = sunpy.map.Map(HMI_LOS_JP2)
-    assert isinstance(jp2_map, sunpy.map.GenericMap)
-    jp2_map.plot()
-    plt.colorbar()
-
-
 def test_map_fits():
     fits_map = sunpy.map.Map(AIA_171_IMAGE, memmap=False)
     assert isinstance(fits_map, sunpy.map.GenericMap)
     # The base of an array that owns its memory is None
     assert fits_map.data.base is None
     fits_map = sunpy.map.Map(AIA_171_IMAGE, memmap=True)
     assert isinstance(fits_map, sunpy.map.GenericMap)
```

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_mapbase.py` & `sunpy-4.1rc1/sunpy/map/tests/test_mapbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         aia171_test_map.coordinate_system.axis1, aia171_test_map.coordinate_system.axis2}
     np.testing.assert_allclose(wcs.wcs.pc, aia171_test_map.rotation_matrix)
 
 
 def test_wcs_cache(aia171_test_map):
     wcs1 = aia171_test_map.wcs
     wcs2 = aia171_test_map.wcs
-    # Check that without any changes to the header, retrieving the wcs twice
+    # Check that without any changes to the header, retreiving the wcs twice
     # returns the same object instead of recomputing the wcs
     assert wcs1 is wcs2
 
     # Change the header and make sure the wcs is re-computed
     new_crpix = 20
     assert new_crpix != wcs2.wcs.crpix[0]
     aia171_test_map.meta['crpix1'] = new_crpix
@@ -317,29 +317,29 @@
 def test_rotation_matrix_cd_cdelt():
     data = np.ones([6, 6], dtype=np.float64)
     header = {
         'CRVAL1': 0,
         'CRVAL2': 0,
         'CRPIX1': 5,
         'CRPIX2': 5,
-        'CDELT1': 2,
-        'CDELT2': 3,
-        'CD1_1': 1,
-        'CD1_2': -2,
-        'CD2_1': 3,
-        'CD2_2': 6,
+        'CDELT1': 10,
+        'CDELT2': 9,
+        'CD1_1': 0,
+        'CD1_2': -9,
+        'CD2_1': 10,
+        'CD2_2': 0,
         'NAXIS1': 6,
         'NAXIS2': 6,
         'CUNIT1': 'arcsec',
         'CUNIT2': 'arcsec',
         'CTYPE1': 'HPLN-TAN',
         'CTYPE2': 'HPLT-TAN',
     }
     cd_map = sunpy.map.Map((data, header))
-    np.testing.assert_allclose(cd_map.rotation_matrix, np.array([[0.5, -1.], [1., 2.]]))
+    np.testing.assert_allclose(cd_map.rotation_matrix, np.array([[0., -1.], [1., 0]]))
 
 
 def test_rotation_matrix_cd_cdelt_square():
     data = np.ones([6, 6], dtype=np.float64)
     header = {
         'CRVAL1': 0,
         'CRVAL2': 0,
@@ -682,37 +682,28 @@
 
 @pytest.mark.parametrize('sample_method, new_dimensions', resample_test_data)
 def test_resample_metadata(generic_map, sample_method, new_dimensions):
     """
     Check that the resampled map has correctly adjusted metadata.
     """
     resampled_map = generic_map.resample(new_dimensions, method=sample_method)
-
-    scale_x = generic_map.data.shape[1] / resampled_map.data.shape[1]
-    scale_y = generic_map.data.shape[0] / resampled_map.data.shape[0]
-
-    assert resampled_map.meta['cdelt1'] == scale_x * generic_map.meta['cdelt1']
-    assert resampled_map.meta['cdelt2'] == scale_y * generic_map.meta['cdelt2']
-    assert resampled_map.meta['pc1_1'] == generic_map.meta['pc1_1']
-    assert resampled_map.meta['pc1_2'] == scale_y / scale_x * generic_map.meta['pc1_2']
-    assert resampled_map.meta['pc2_1'] == scale_x / scale_y * generic_map.meta['pc2_1']
-    assert resampled_map.meta['pc2_2'] == generic_map.meta['pc2_2']
-
+    assert resampled_map.meta['cdelt1'] == generic_map.meta['cdelt1']
+    assert resampled_map.meta['cdelt2'] == generic_map.meta['cdelt2']
     # TODO: we should really test the numbers here, not just that the correct
     # header values have been modified. However, I am lazy and we have figure
     # tests.
     assert resampled_map.meta['crpix1'] != generic_map.meta['crpix1']
     assert resampled_map.meta['crpix2'] != generic_map.meta['crpix2']
     assert u.allclose(resampled_map.meta['crval1'], generic_map.meta['crval1'])
     assert u.allclose(resampled_map.meta['crval2'], generic_map.meta['crval2'])
     assert resampled_map.meta['naxis1'] == new_dimensions[0].value
     assert resampled_map.meta['naxis2'] == new_dimensions[1].value
     for key in generic_map.meta:
-        if key not in ('cdelt1', 'cdelt2', 'pc1_2', 'pc2_1', 'crpix1', 'crpix2', 'crval1',
-                       'crval2', 'naxis1', 'naxis2'):
+        if key not in ('crpix1', 'crpix2', 'crval1',
+                       'crval2', 'naxis1', 'naxis2') and not key.startswith('pc'):
             assert resampled_map.meta[key] == generic_map.meta[key]
 
 
 @pytest.mark.parametrize('sample_method, new_dimensions', resample_test_data)
 def test_resample_simple_map(simple_map, sample_method, new_dimensions):
     # Put the reference pixel at the top-right of the bottom-left pixel
     simple_map.meta['crpix1'] = 1.5
@@ -758,40 +749,14 @@
     assert superpix_map.dimensions[1] == expected_new_dims[1]
 
     # Check value of lower left pixel is calculated correctly
     expected = f(aia171_test_map.data[0:2, 0:2])
     assert_quantity_allclose(superpix_map.data[0, 0], expected)
 
 
-@pytest.mark.parametrize('f, dimensions', [(np.sum, (2, 3)*u.pix),
-                                           (np.mean, (3, 2)*u.pix)])
-def test_superpixel_metadata(generic_map, f, dimensions):
-    superpix_map = generic_map.superpixel(dimensions, func=f)
-
-    scale_x, scale_y = dimensions.value
-
-    assert superpix_map.meta['cdelt1'] == scale_x * generic_map.meta['cdelt1']
-    assert superpix_map.meta['cdelt2'] == scale_y * generic_map.meta['cdelt2']
-    assert superpix_map.meta['pc1_1'] == generic_map.meta['pc1_1']
-    assert superpix_map.meta['pc1_2'] == scale_y / scale_x * generic_map.meta['pc1_2']
-    assert superpix_map.meta['pc2_1'] == scale_x / scale_y * generic_map.meta['pc2_1']
-    assert superpix_map.meta['pc2_2'] == generic_map.meta['pc2_2']
-
-    assert superpix_map.meta['crpix1'] - 0.5 == (generic_map.meta['crpix1'] - 0.5) / scale_x
-    assert superpix_map.meta['crpix2'] - 0.5 == (generic_map.meta['crpix2'] - 0.5) / scale_y
-    assert u.allclose(superpix_map.meta['crval1'], generic_map.meta['crval1'])
-    assert u.allclose(superpix_map.meta['crval2'], generic_map.meta['crval2'])
-    assert superpix_map.meta['naxis1'] == generic_map.meta['naxis1'] / scale_x
-    assert superpix_map.meta['naxis2'] == generic_map.meta['naxis2'] / scale_y
-    for key in generic_map.meta:
-        if key not in ('cdelt1', 'cdelt2', 'pc1_2', 'pc2_1', 'crpix1', 'crpix2', 'crval1',
-                       'crval2', 'naxis1', 'naxis2'):
-            assert superpix_map.meta[key] == generic_map.meta[key]
-
-
 def test_superpixel_masked(aia171_test_map_with_mask):
     input_dims = u.Quantity(aia171_test_map_with_mask.dimensions)
     dimensions = (2, 2) * u.pix
     # Test that the mask is respected
     superpix_map = aia171_test_map_with_mask.superpixel(dimensions)
     assert superpix_map.mask is not None
     # Check the shape of the mask
@@ -848,16 +813,14 @@
 @pytest.mark.parametrize('method', ['resample', 'superpixel'])
 @settings(max_examples=10, deadline=1000)
 @given(cd=matrix_meta('cd'))
 def test_resample_rotated_map_cd(cd, method):
     smap = make_simple_map()
 
     smap.meta.update(cd)
-    for key in ['cdelt1', 'cdelt2', 'pc1_1', 'pc1_2', 'pc2_1', 'pc2_2']:
-        del smap.meta[key]
     # Check superpixel with a rotated map with unequal resampling
     new_dims = (1, 2) * u.pix
     new_map = getattr(smap, method)(new_dims)
     # Coordinate of the lower left corner should not change
     ll_pix = [-0.5, -0.5]*u.pix
     assert smap.pixel_to_world(*ll_pix).separation(
         new_map.pixel_to_world(*ll_pix)).to(u.arcsec) < 1e-8 * u.arcsec
@@ -1252,15 +1215,14 @@
 
     inputs = (
         ((bl_coord,), dict(top_right=tr_coord)),
         ((bl_coord,), dict(width=width_deg, height=height_deg)),
         ((bl_tr_coord,), {}),
         ((bl_pix,), dict(top_right=tr_pix)),
         ((bl_pix,), dict(width=width_pix, height=height_pix)),
-        ((bl_tr_coord.frame,), {}),
     )
 
     for args, kwargs in inputs:
         smap = generic_map2.submap(*args, **kwargs)
         assert u.allclose(smap.dimensions, (3, 3) * u.pix)
 
 
@@ -1462,15 +1424,14 @@
     fig = Figure(figsize=(8, 4))
 
     ax1 = fig.add_subplot(121, projection=weird_map)
     weird_map.plot(axes=ax1, title='Map with a non-pure-rotation PCij matrix')
 
     ax2 = fig.add_subplot(122, projection=derotated_map)
     derotated_map.plot(axes=ax2, title=f'De-rotated map via {method}')
-    ax2.set_aspect(derotated_map.scale[1] / derotated_map.scale[0])
 
     return fig
 
 
 # This function is used in the arithmetic tests below
 def check_arithmetic_value_and_units(map_new, data_expected):
     assert u.allclose(map_new.quantity, data_expected)
@@ -1549,30 +1510,7 @@
 def test_parse_fits_units():
     # Check that we parse a BUNIT of G correctly.
     out_unit = GenericMap._parse_fits_unit("Gauss")
     assert out_unit == u.G
 
     out_unit = GenericMap._parse_fits_unit("G")
     assert out_unit == u.G
-
-
-def test_only_cd():
-    data = np.ones([6, 6], dtype=np.float64)
-    header = {
-        'CRVAL1': 0,
-        'CRVAL2': 0,
-        'CRPIX1': 5,
-        'CRPIX2': 5,
-        'CD1_1': 3,
-        'CD1_2': -4,
-        'CD2_1': 5,
-        'CD2_2': 12,
-        'NAXIS1': 6,
-        'NAXIS2': 6,
-        'CUNIT1': 'arcsec',
-        'CUNIT2': 'arcsec',
-        'CTYPE1': 'HPLN-TAN',
-        'CTYPE2': 'HPLT-TAN',
-    }
-    cd_map = sunpy.map.Map((data, header))
-    np.testing.assert_allclose(u.Quantity(cd_map.scale).value, np.array([5, 13]))
-    np.testing.assert_allclose(cd_map.rotation_matrix, np.array([[3/5, -4/5], [5/13, 12/13]]))
```

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_mapsequence.py` & `sunpy-4.1rc1/sunpy/map/tests/test_mapsequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     assert np.all(np.asarray([isinstance(h, MetaDict) for h in meta]))
     assert np.all(np.asarray(
         [meta[i] == mapsequence_all_the_same[i].meta for i in range(0, len(meta))]))
 
 
 def test_repr(mapsequence_all_the_same, mapsequence_different_maps):
     """
-    Tests that overridden __repr__ functionality works as expected. Test
+    Tests that overidden __repr__ functionality works as expected. Test
     for mapsequence of same maps as well that of different maps.
     """
     # Test the case of MapSequence having same maps
     expected_out = f'MapSequence of 2 elements, with maps from AIAMap'
     obtained_out = repr(mapsequence_all_the_same)
     assert obtained_out.startswith(object.__repr__(mapsequence_all_the_same))
     assert len(mapsequence_all_the_same) == 2
```

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_maputils.py` & `sunpy-4.1rc1/sunpy/map/tests/test_maputils.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_plotting.py` & `sunpy-4.1rc1/sunpy/map/tests/test_plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 @figure_test
 def test_quadrangle_aia17_width_height(aia171_test_map):
     aia171_test_map.plot()
     bottom_left = SkyCoord(
         50 * u.deg, -10 * u.deg, frame=HeliographicStonyhurst, obstime=aia171_test_map.date)
     w = 30 * u.deg
     h = 90 * u.deg
-    aia171_test_map.draw_quadrangle(bottom_left=bottom_left.frame, width=w, height=h)
+    aia171_test_map.draw_quadrangle(bottom_left=bottom_left, width=w, height=h)
 
 
 @figure_test
 def test_quadrangle_aia17_pix_width_height(aia171_test_map):
     aia171_test_map.plot()
     aia171_test_map.draw_quadrangle(bottom_left=(50, 50)*u.pix, width=30*u.pix,
                                     height=50*u.pix, edgecolor="cyan")
@@ -341,29 +341,7 @@
     rotated_map.plot(axes=ax, autoalign=True)
     return fig
 
 
 def test_plot_autoalign_bad_inputs(aia171_test_map):
     with pytest.raises(ValueError):
         aia171_test_map.plot(autoalign='bad')
-
-
-@figure_test
-def test_plot_autoalign_pixel_alignment(aia171_test_map):
-    # Verify that autoalign=True does not affect pixel alignment
-    x, y = [z.value for z in aia171_test_map.reference_pixel]
-
-    fig = Figure(figsize=(10, 4))
-
-    ax1 = fig.add_subplot(121, projection=aia171_test_map)
-    aia171_test_map.plot(axes=ax1, autoalign=False, title='autoalign=False')
-    ax1.grid(False)
-    ax1.set_xlim(x - 2, x + 2)
-    ax1.set_ylim(y - 2, y + 2)
-
-    ax2 = fig.add_subplot(122, projection=aia171_test_map)
-    aia171_test_map.plot(axes=ax2, autoalign=True, title='autoalign=True')
-    ax2.grid(False)
-    ax2.set_xlim(x - 2, x + 2)
-    ax2.set_ylim(y - 2, y + 2)
-
-    return fig
```

### Comparing `sunpy-4.1.5/sunpy/map/tests/test_reproject_to.py` & `sunpy-4.1rc1/sunpy/map/tests/test_reproject_to.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/_attrs.py` & `sunpy-4.1rc1/sunpy/net/_attrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         # Note: the website asks for GHz, however it seems that using GHz
         # produces weird responses on VSO.
         supported_units = [u.AA, u.kHz, u.keV]
         for unit in supported_units:
             if wavemin.unit.is_equivalent(unit):
                 break
         else:
-            raise u.UnitsError(f"This unit is not convertible to any of {supported_units}")
+            raise u.UnitsError(f"This unit is not convertable to any of {supported_units}")
 
         wavemin, wavemax = sorted([wavemin.to(unit), wavemax.to(unit)])
         self.unit = unit
 
         super().__init__(wavemin, wavemax)
 
     def collides(self, other):
```

### Comparing `sunpy-4.1.5/sunpy/net/attr.py` & `sunpy-4.1rc1/sunpy/net/attr.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/attrs.py` & `sunpy-4.1rc1/sunpy/net/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/base_client.py` & `sunpy-4.1rc1/sunpy/net/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
                 raise NameError(f"{name} has already been registered as an attrs name.")
 
             setattr(attrs, name, module_obj)
 
             if name not in attrs.__all__:
                 attrs.__all__.append(name)
 
-        # Register client attrs after it has registered its own attrs
+        # Register client attrs after it has regsitered its own attrs
         from sunpy.net import attr
         values = cls.register_values()
         # If the client has no support, we won't try to register attrs
         if values:
             attr.Attr.update_values({cls: values})
 
     def __repr__(self):
```

### Comparing `sunpy-4.1.5/sunpy/net/cdaweb/cdaweb.py` & `sunpy-4.1rc1/sunpy/net/cdaweb/cdaweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     SOLO_L2_MAG-RTN-NORMAL-1-MINUTE 2021-07-07 00:00:29.000 2021-07-07 23:59:30.000
     <BLANKLINE>
     <BLANKLINE>
 
     See Also
     --------
     sunpy.net.cdaweb.get_datasets : Find dataset IDs for a given observatory
-    sunpy.net.cdaweb.get_observatory_groups : Get all observatories available from CDAWeb
+    sunpy.net.cdaweb.get_observatory_groups : Get all observatories avaiable from CDAWeb
     """
     @property
     def info_url(self):
         return 'https://cdaweb.gsfc.nasa.gov/index.html'
 
     def search(self, *query, **kwargs):
         """
```

### Comparing `sunpy-4.1.5/sunpy/net/cdaweb/data/attrs.json` & `sunpy-4.1rc1/sunpy/net/cdaweb/data/attrs.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9467994913098771%*

 * *Differences: {"'ELA_L1_STATE_DEFN'": "'Probe state file, contains definitive position, attitude and orbit "*

 * *                        "events - V. Angelopoulos (UCLA, IGPP/EPSS)'",*

 * * "'ELA_L1_STATE_PRED'": "'Probe state file, contains predictive position, velocity, and attitude - "*

 * *                        "V. Angelopoulos (UCLA, IGPP/EPSS)'",*

 * * "'ELB_L1_STATE_DEFN'": "'Probe state file, contains definitive position, attitude and orbit "*

 * *                        "events - V. Angelopoulos (UCLA, IGPP/EPSS)'",*

 * * "'ELB_L1_STATE_P […]*

```diff
@@ -32,15 +32,14 @@
     "AC_K1_MFI": "ACE Magnetic Field 16-Second Key Parameters [PRELIM] - N. Ness (Bartol Research Institute)",
     "AC_K1_SWE": "K1 - ACE Solar Wind Experiment 1-Hour Key Parameters [PRELIM] - D. J. McComas (Southwest Research Institute)",
     "AC_K2_MFI": "K2 - ACE Magnetic Field 1-Hour Key Parameters [PRELIM] - N. Ness (Bartol Research Institute)",
     "AC_OR_DEF": "ACE Daily GSE and J2000 GCI Position Data - E. C. Stone (California Institute of Technology)",
     "AC_OR_SSC": "ACE GSE Positions @ 12 min resolution  - SSC/SSCWeb ( NASA's GSFC)",
     "AEROCUBE-6-A_DOSIMETER_L2": "Aerocube 6/Dosimeter Level 2 - J. B. Blake (The Aerospace Corporation)",
     "AEROCUBE-6-B_DOSIMETER_L2": "Aerocube 6/Dosimeter Level 2 - J. B. Blake (The Aerospace Corporation)",
-    "AIM_CIPS_SCI_3A": "AIM Cloud Imaging and Particle Size (CIPS) Polar Mesospheric Clouds (PMC) Daily Images - Cora E. Randall (University of Colorado)",
     "ALOUETTE2_AV_LIM": "Alouette-2 Topside Sounder Ionograms over Lima, Peru (Lat=-12, Long=283) - R.F. Benson (NASA GSFC)",
     "ALOUETTE2_AV_QUI": "Alouette-2 Topside Sounder Ionogram over Quito, Equador (lat/lon=-1/281) - R.F. Benson (NASA GSFC)",
     "ALOUETTE2_AV_SNT": "Alouette-2 Topside Sounder Ionogram over Santiago, Chile (lat/lon=-33/298) - R.F. Benson (NASA GSFC)",
     "ALOUETTE2_AV_SOL": "Alouette-2 Topside Sounder Ionogram over Falkland Is., U.K. (lat/lon=-52/302) - R.F. Benson (NASA GSFC)",
     "ALOUETTE2_AV_ULA": "Alouette-2 Topside Sounder Ionogram over Fairbanks, Alaska (lat/long=65/212) - R.F. Benson (NASA GSFC)",
     "ALOUETTE2_AV_WNK": "Alouette-2 Topside Sounder Ionogram over Winkfield, U.K. (lat/lon=51/359) - R.F. Benson (NASA GSFC)",
     "ALOUETTE2_NEPROF_TOPS": "Alouette-2 CRC Electron Density Profiles - J. E. Jackson (Communication Research Centre (CRC), Ottawa)",
@@ -433,59 +432,51 @@
     "C1_PP_EDI": "Cluster Spacecraft 1, EDI Prime Parameters - G. Paschmann (MPE)",
     "C1_PP_EFW": "Cluster Spacecraft 1, EFW Prime Parameters - G. Gustafsson (IRFU)",
     "C1_PP_PEA": "Cluster Spacecraft 1, PEACE Prime Parameters - A. Fazakerley (MSSL)",
     "C1_PP_RAP": "Cluster Spacecraft 1, RAPID Prime Parameters - B. Wilken and P. Daly (MPAe)",
     "C1_PP_STA": "Cluster Spacecraft 1, STAFF Prime Parameters - N. Cornilleau-Wehrlin (CETP)",
     "C1_PP_WHI": "Cluster Spacecraft 1, WHISPER Prime Parameters - P.M.E. Decreau (LPCE)",
     "C1_UP_FGM": "Cluster Spacecraft 1, FluxGate Magnetometer (FGM) Unvalidated Prime Parameters - A. Balogh (ICSTM)",
-    "C1_WAVEFORM_WBD": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
-    "C1_WAVEFORM_WBD_BM2": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
     "C2_CP_FGM_SPIN": "Cluster Spacecraft 2 FluxGate Magnetometer (FGM) Spin-Resolution Parameters - Andre Balogh>a.balogh@imperial.ac.uk & Elizabeth Lucek>e.lucek@imperial.ac.uk & ESA CAA (Imperial College)",
     "C2_JP_PMP": "Cluster Spacecraft 2, JSOC Predicted Magnetic Positions - M. Hapgood (RAL)",
     "C2_JP_PSE": "Cluster Spacecraft 2, JSOC Predicted Scientific Events - M. Hapgood (RAL)",
     "C2_PP_ASP": "Cluster Spacecraft 2, ASPOC Prime Parameters - W. Riedler (IWF-OAW)",
     "C2_PP_DWP": "Cluster Spacecraft 2, DWP Prime Parameters - H. Alleyne (Univ-Sheff)",
     "C2_PP_EDI": "Cluster Spacecraft 2, EDI Prime Parameters - G. Paschmann (MPE)",
     "C2_PP_EFW": "Cluster Spacecraft 2, EFW Prime Parameters - G. Gustafsson (IRFU)",
     "C2_PP_PEA": "Cluster Spacecraft 2, PEACE Prime Parameters - A. Fazakerley (MSSL)",
     "C2_PP_RAP": "Cluster Spacecraft 2, RAPID Prime Parameters - B. Wilken and P. Daly (MPAe)",
     "C2_PP_STA": "Cluster Spacecraft 2, STAFF Prime Parameters - N. Cornilleau-Wehrlin (CETP)",
     "C2_PP_WHI": "Cluster Spacecraft 2, WHISPER Prime Parameters - P.M.E. Decreau (LPCE)",
     "C2_UP_FGM": "Cluster Spacecraft 2, FluxGate Magnetometer (FGM) Unvalidated Prime Parameters - A. Balogh (ICSTM)",
-    "C2_WAVEFORM_WBD": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
-    "C2_WAVEFORM_WBD_BM2": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
     "C3_CP_FGM_SPIN": "Cluster Spacecraft 3 FluxGate Magnetometer (FGM) Spin-Resolution Parameters - Andre Balogh>a.balogh@imperial.ac.uk & Elizabeth Lucek>e.lucek@imperial.ac.uk & ESA CAA (Imperial College)",
     "C3_JP_PMP": "Cluster Spacecraft 3, JSOC Predicted Magnetic Positions - M. Hapgood (RAL)",
     "C3_JP_PSE": "Cluster Spacecraft 3, JSOC Predicted Scientific Events - M. Hapgood (RAL)",
     "C3_PP_ASP": "Cluster Spacecraft 3, ASPOC Prime Parameters - W. Riedler (IWF-OAW)",
     "C3_PP_CIS": "Cluster Spacecraft 3, CIS Prime Parameters - H. Reme (CESR)",
     "C3_PP_EDI": "Cluster Spacecraft 3, EDI Prime Parameters - G. Paschmann (MPE)",
     "C3_PP_EFW": "Cluster Spacecraft 3, EFW Prime Parameters - G. Gustafsson (IRFU)",
     "C3_PP_PEA": "Cluster Spacecraft 3, PEACE Prime Parameters - A. Fazakerley (MSSL)",
     "C3_PP_RAP": "Cluster Spacecraft 3, RAPID Prime Parameters - B. Wilken and P. Daly (MPAe)",
     "C3_PP_STA": "Cluster Spacecraft 3, STAFF Prime Parameters - N. Cornilleau-Wehrlin (CETP)",
     "C3_PP_WHI": "Cluster Spacecraft 3, WHISPER Prime Parameters - P.M.E. Decreau (LPCE)",
     "C3_UP_FGM": "Cluster Spacecraft 3, FluxGate Magnetometer (FGM) Unvalidated Prime Parameters - A. Balogh (ICSTM)",
-    "C3_WAVEFORM_WBD": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
-    "C3_WAVEFORM_WBD_BM2": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
     "C4_CP_FGM_SPIN": "Cluster Spacecraft 4 FluxGate Magnetometer (FGM) Spin-Resolution Parameters - Andre Balogh>a.balogh@imperial.ac.uk & Elizabeth Lucek>e.lucek@imperial.ac.uk & ESA CAA (Imperial College)",
     "C4_JP_PMP": "Cluster Spacecraft 4, JSOC Predicted Magnetic Positions - M. Hapgood (RAL)",
     "C4_JP_PSE": "Cluster Spacecraft 4, JSOC Predicted Scientific Events - M. Hapgood (RAL)",
     "C4_PP_ASP": "Cluster Spacecraft 4, ASPOC Prime Parameters - W. Riedler (IWF-OAW)",
     "C4_PP_CIS": "Cluster Spacecraft 4, CIS Prime Parameters - H. Reme (CESR)",
     "C4_PP_DWP": "Cluster Spacecraft 4, DWP Prime Parameters - H. Alleyne (Univ-Sheff)",
     "C4_PP_EDI": "Cluster Spacecraft 4, EDI Prime Parameters - G. Paschmann (MPE)",
     "C4_PP_EFW": "Cluster Spacecraft 4, EFW Prime Parameters - G. Gustafsson (IRFU)",
     "C4_PP_PEA": "Cluster Spacecraft 4, PEACE Prime Parameters - A. Fazakerley (MSSL)",
     "C4_PP_RAP": "Cluster Spacecraft 4, RAPID Prime Parameters - B. Wilken and P. Daly (MPAe)",
     "C4_PP_STA": "Cluster Spacecraft 4, STAFF Prime Parameters - N. Cornilleau-Wehrlin (CETP)",
     "C4_PP_WHI": "Cluster Spacecraft 4, WHISPER Prime Parameters - P.M.E. Decreau (LPCE)",
     "C4_UP_FGM": "Cluster Spacecraft 4, FluxGate Magnetometer (FGM) Unvalidated Prime Parameters - A. Balogh (ICSTM)",
-    "C4_WAVEFORM_WBD": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
-    "C4_WAVEFORM_WBD_BM2": "Cluster Wideband Data Plasma Wave Receiver/High Time Resolution Waveform Data - 2006 - Current:  J. S. Pickett; 1988 - 2006:  D. A. Gurnett (The University of  Iowa)",
     "CASSINI_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "CASSINI_MAG_1MIN_MAGNETIC_FIELD": "1 min averaged magnetic field - Michele Dougherty (Imperial College, London)",
     "CL_JP_PCY": "Cluster, Monthly JSOC Predicted Solar Cycle Trends - M. Hapgood (RAL)",
     "CL_JP_PGP": "Cluster, JSOC Predicted Geometric Positions - M. Hapgood (RAL)",
     "CL_OR_GIFWALK": "Link to Cluster orbit plots - Polar-Wind-Geotail Ground System (NASA GSFC)",
     "CL_SP_AUX": "Cluster, Auxiliary  Parameters - Hungarian Data Centre/M. Tatrallyay (KFKI)",
     "CNOFS_CINDI_IVM_500MS": "CNOFS CINDI IVM ion density, composition, temperature, and drift (0.5-sec) - Dr. Roderick A. Heelis (University of Texas, Dallas)",
@@ -557,20 +548,19 @@
     "DSCOVR_AT_DEF": "DSCOVR Definitive Attitude - A. Szabo (NASA Goddard Space Flight Center)",
     "DSCOVR_AT_PRE": "DSCOVR Preliminary Attitude - A. Szabo (NASA Goddard Space Flight Center)",
     "DSCOVR_H0_MAG": "DSCOVR Fluxgate Magnetometer 1-sec Definitive Data - A. Koval (UMBC, NASA/GSFC)",
     "DSCOVR_H1_FC": "Isotropic Maxwellian parameters for solar wind protons. - Justin C. Kasper (Smithonian Astrophysical Observatory)",
     "DSCOVR_ORBIT_PRE": "DSCOVR Predicted Orbit - A. Szabo (NASA Goddard Space Flight Center)",
     "EARTH_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "ELA_L1_EPDEF": "Energetic Particle Detector, Counts, Electrons>keV [UNCALIBRATED RAW DATA]  - V. Angelopoulos (UCLA, IGPP/EPSS)",
-    "ELA_L1_STATE_DEFN": "ELFIN-A state file, contains definitive position, attitude and orbit events - V. Angelopoulos (UCLA, IGPP/EPSS)",
-    "ELA_L1_STATE_PRED": "ELFIN-A state file, contains predictive position, velocity, and attitude - V. Angelopoulos (UCLA, IGPP/EPSS)",
+    "ELA_L1_STATE_DEFN": "Probe state file, contains definitive position, attitude and orbit events - V. Angelopoulos (UCLA, IGPP/EPSS)",
+    "ELA_L1_STATE_PRED": "Probe state file, contains predictive position, velocity, and attitude - V. Angelopoulos (UCLA, IGPP/EPSS)",
     "ELB_L1_EPDEF": "Energetic Particle Detector, Counts, Electrons>keV [UNCALIBRATED RAW DATA]  - V. Angelopoulos (UCLA, IGPP/EPSS)",
-    "ELB_L1_STATE_DEFN": "ELFIN-B state file, contains definitive position, attitude and orbit events - V. Angelopoulos (UCLA, IGPP/EPSS)",
-    "ELB_L1_STATE_PRED": "ELFIN-B state file, contains predictive position, velocity, and attitude - V. Angelopoulos (UCLA, IGPP/EPSS)",
-    "ENDURANCE_EPHEMERIS_DEF": "Position and attitude of Endurance during flight - G. Collinson (NASA GSFC / Catholic University of America)",
+    "ELB_L1_STATE_DEFN": "Probe state file, contains definitive position, attitude and orbit events - V. Angelopoulos (UCLA, IGPP/EPSS)",
+    "ELB_L1_STATE_PRED": "Probe state file, contains predictive position, velocity, and attitude - V. Angelopoulos (UCLA, IGPP/EPSS)",
     "EQ_PP_AUX": "Equator-S Auxiliary Data Prime Parameters -  EDC (MPE)",
     "EQ_PP_EDI": "Equator-S Electron Drift Instrument Prime Parameters - G. Paschmann (MPE)",
     "EQ_PP_EPI": "Equator-S Energetic Particle Instrument Prime Parameters - T. Sanderson (ESTEC)",
     "EQ_PP_ICI": "Equator-S Ion Composition Instrument Prime Parameters.(The raw moments calculated onboard should only be used qualitatively for identifying regions and temporal variations. Quantitative analysis should be done with the final moments generated from telemetered 3D distributions.) - L. Kistler (UNH)",
     "EQ_PP_MAM": "Equator-S Fluxgate Magnetometer Prime Parameters - W. Baumjohann (MPE)",
     "EQ_PP_PCD": "Equator-S Potential Control Device Prime Parameters - K. Torkar (IWF)",
     "EQ_SP_SFD": "Equator-S Scintillating Fibre Detector Summary Parameters - L. Adams (ESTEC)",
@@ -696,15 +686,14 @@
     "HELIOS2_E6_KUNOW_1HOUR_PARTICLE-FLUX": "Hourly averaged fluxes of e, H and He from Helios-1/E6(Kunow) -  H. Kunow (University of Kiel)",
     "HELIOS2_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "HK_H0_MAG": "Hawkeye Magnetic Field Instrument - J. Van Allen (University of Iowa)",
     "HK_H0_VLF": "Hk Electric and Magnetic Field Radio Frequency Spectrum Analyzer High Time Resolution - D. Gurnett (University of Iowa)",
     "HYAKUTAKE_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "I1_AV2_OTT": "ISIS Topside Sounder Ionogram - R.F. Benson (NASA GSFC)",
     "I1_AV2_QUI": "ISIS Topside Sounder Ionogram - R.F. Benson (NASA GSFC)",
-    "I1_AV2_SNT": "ISIS Topside Sounder Ionogram - R.F. Benson (NASA GSFC)",
     "I1_AV2_ULA": "ISIS Topside Sounder Ionogram - R.F. Benson (NASA GSFC)",
     "I1_AV_ALL": "ISIS-1 Topside sounder ionograms, all stations merged into a single dataset - R.F. Benson (NASA GSFC)",
     "I1_AV_KER": "ISIS-1 Topside Sounder Ionograms over Kerguelen Island, France (Lat=-49, Long=70) - R.F. Benson (NASA GSFC)",
     "I1_AV_KSH": "ISIS-1 Topside Sounder Ionogram over Kashima, Japan (lat/lon=36/141) - R.F. Benson (NASA GSFC)",
     "I1_AV_KWA": "ISIS-1 Topside Sounder Ionogram over Kwajalein, Marshall Is. (lat/lon=9/168) - R.F. Benson (NASA GSFC)",
     "I1_AV_ODG": "ISIS-1 Topside Sounder Ionogram over Ouagadougou, Burkina Faso (lat/lon=14/359) - R.F. Benson (NASA GSFC)",
     "I1_AV_ORR": "ISIS-1 Topside Sounder Ionogram over Orroral, Australia (lat/lon=-36/149) - R.F. Benson (NASA GSFC)",
@@ -756,49 +745,14 @@
     "IA_K0_MFI": "Interball Auroral probe Magnetic Field, Key Parameters - V.Petrov (IMAP:IZMIRAN,Troitsk,  Russia. )",
     "IA_OR_DEF": "Interball Auroral Probe Orbital Data, Key Parameters - V.Prokhorenko (Space Research Inst., Russian Acad. Sci., Moscow, Russia. )",
     "IBEX_H3_ENA_HI_R04_DEFLECTION_1AU_7DAY": "IBEX-Hi Release 4; Survival Probabilities tables - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R04_DEFLECTION_SCF_7DAY": "IBEX-Hi Release 4; Survival Probabilities tables - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R04_LOSS_1AU_7DAY": "IBEX-Hi Release 4; Survival Probabilities tables - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R04_LOSS_SCF_7DAY": "IBEX-Hi Release 4; Survival Probabilities tables - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R04_SURVPRO_SCF_7DAY": "IBEX-Hi Release 4; Survival Probabilities tables - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_ANTIRAM_MIF_5YR": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Antiram-directional 1-to-5-year Average West Ecliptic Maps in Mono Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_ANTIRAM_VEIF_5YR": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Antiram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_OMNI_6MO": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_OMNI_MIF_10MP": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Omnidirectional 1-to-10-map Average West Ecliptic Maps in Mono Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_OMNI_VEIF_10MP": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Omnidirectional 1-to-10-map Average West Ecliptic Maps in Var Energy Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_RAM_1YR": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_RAM_MIF_5YR": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Ram-directional 1-to-5-year Average West Ecliptic Maps in Mono Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_NOSP_RAM_VEIF_5YR": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Ram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_ANTIRAM_1YR": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, ANTIRAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_ANTIRAM_MIF_5YR": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, Antiram-directional 1-to-5-year Average West Ecliptic Maps in Mono Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_ANTIRAM_VEIF_5YR": "IBEX-Hi Release 7; Compton-Getting, no Survival-Probability, Antiram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_OMNI_6MO": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_OMNI_MIF_10MP": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, Omnidirectional 1-to-10 map Average West Ecliptic Maps in Mono Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_OMNI_VEIF_10MP": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, Omnidirectional 1-to-10-map Average West Ecliptic Maps in Var Energy Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_RAM_1YR": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_RAM_MIF_5YR": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, Ram-directional 1-to-5-year Average West Ecliptic Maps in Mono Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_CG_SP_RAM_VEIF_5YR": "IBEX-Hi Release 7; Compton-Getting, Survival-Probability, Ram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_NOSP_ANTIRAM_1YR": "IBEX-Hi Release 7; no Compton-Getting, no Survival-Probability, ANTIRAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_NOSP_ANTIRAM_VESCF_5YR": "IBEX-Hi Release 7; no Compton-Getting, no Survival-Probability, Antiram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy SC Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_NOSP_OMNI_6MO": "IBEX-Hi Release 7; no Compton-Getting, no Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_NOSP_OMNI_VESCF_10MP": "IBEX-Hi Release 7; no Compton-Getting, no Survival-Probability, Omnidirectional 1-to-10-map Average West Ecliptic Maps in Var Energy SC Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_NOSP_RAM_1YR": "IBEX-Hi Release 7; no Compton-Getting, no Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_NOSP_RAM_VEIF_5YR": "IBEX-Hi Release 7; no Compton-Getting, no Survival-Probability, Ram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy Inertial Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_SP_ANTIRAM_1YR": "IBEX-Hi Release 7; no Compton-Getting, Survival-Probability, ANTIRAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_SP_ANTIRAM_VESCF_5YR": "IBEX-Hi Release 7; no Compton-Getting, no Survival-Probability, Antiram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy SC Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_SP_OMNI_6MO": "IBEX-Hi Release 7; no Compton-Getting, Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_SP_OMNI_VESCF_10MP": "IBEX-Hi Release 7; no Compton-Getting, Survival-Probability, Omnidirectional 1-to-10-map Average West Ecliptic Maps in Var Energy SC Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_SP_RAM_1YR": "IBEX-Hi Release 7; no Compton-Getting, Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R07_NOCG_SP_RAM_VESCF_5YR": "IBEX-Hi Release 7; no Compton-Getting, Survival-Probability, Ram-directional 1-to-5-year Average West Ecliptic Maps in Var Energy SC Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R08_OMNI_F2-RIBBON-MAPS-GAL_5YR": "IBEX-Hi Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R08_OMNI_F2-RIBBON-MAPS-J2000_5YR": "IBEX-Hi Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R08_OMNI_F2-RIBBON-MAPS_5YR": "IBEX-Hi Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R08_OMNI_F3-GDF-MAPS-GALACTIC_5YR": "IBEX-Hi Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R08_OMNI_F3-GDF-MAPS-J2000_5YR": "IBEX-Hi Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R08_OMNI_F3-GDF-MAPS_5YR": "IBEX-Hi Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_CG_NOSP_ANTIRAM_1YR": "IBEX-Hi Release-10; Compton-Getting, no Survival-Probability, antiram-direction 1-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_CG_NOSP_ANTIRAM_7YR": "IBEX-Hi Release-10; Compton-Getting, no Survival-Probability, antiram-direction 7-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_CG_NOSP_OMNI_6MO": "IBEX-Hi Release-10; Compton-Getting, no Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_CG_NOSP_OMNI_7YR": "IBEX-Hi Release-10; Compton-Getting, no Survival-Probability, omni-direction 7-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_CG_NOSP_RAM_1YR": "IBEX-Hi Release-10; Compton-Getting, no Survival-Probability, ram-direction 1-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_CG_NOSP_RAM_7YR": "IBEX-Hi Release-10; Compton-Getting, no Survival-Probability, ram-direction 7-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_CG_SP_ANTIRAM_1YR": "IBEX-Hi Release-10; Compton-Getting, Survival-Probability, AntiRAMdirectional 1-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
@@ -817,83 +771,32 @@
     "IBEX_H3_ENA_HI_R10_NOCG_SP_OMNI_6MO": "IBEX-Hi Release-10; no Compton-Getting, Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_NOCG_SP_OMNI_7YR": "IBEX-Hi Release-10; no Compton-Getting, Survival-Probability, omni-direction 7-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R10_NOCG_SP_RAM_1YR": "IBEX-Hi Release-10; no Compton-Getting, Survival-Probability, ram-direction 1-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R12_MAGNETOSPHERE_24MIN": "IBEX-Hi Release-12; Count Data for Magnetospheric Imaging.  - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R13_CG_NOSP_ANTIRAM_1YR": "IBEX-Hi Release-13; Compton-Getting, no Survival-Probability, antiram-direction 1-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R13_CG_NOSP_RAM_1YR": "IBEX-Hi Release-13; Compton-Getting, no Survival-Probability, ram-direction 1-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_HI_R14_PRESS-SLOPE_CG_NOSP_RAM_3YR": "IBEX-Hi Release-14; Compton-Getting, no Survival-Probability, ram-direction 3-year-Average West Ecliptic Pressure andFlux Power-Law Slope Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R15_CG_SP_RIBCEN_1YR": "IBEX-Hi Release 15; Compton-Getting, Survival-Probability, in a ribbon centered frame, 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R15_CG_SP_RIBCEN_2YR": "IBEX-Hi Release 15; Compton-Getting, Survival-Probability, in a ribbon centered frame, 2-Year-Averaged West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R15_CG_SP_RIBCEN_3YR": "IBEX-Hi Release 15; Compton-Getting, Survival-Probability, in a ribbon centered frame, 3-Year-Averaged West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_NOSP_OMNI_11YR": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, Omnidirectional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_NOSP_OMNI_6MO": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_NOSP_RAM_11YR": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, ram-directional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_NOSP_RAM_1YR": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_ANTIRAM_11YR": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, Antiram-directional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_ANTIRAM_1YR": "IBEX-Hi Release 16; Compton-Getting, Survival-Probability, ANTIRAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_OMNI_11YR": "IBEX-Hi Release 16; Compton-Getting, Survival-Probability, Omnidirectional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_OMNI_2YR": "IBEX-Hi Release 16; Compton-Getting, Survival-Probability, Omnidirectional 2-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_OMNI_3YR": "IBEX-Hi Release 16; Compton-Getting, Survival-Probability, Omnidirectional 3-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_OMNI_6MO": "IBEX-Hi Release 16; Compton-Getting, Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_RAM_11YR": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, Ram-directional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_CG_SP_RAM_1YR": "IBEX-Hi Release 16; Compton-Getting, Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_NOSP_ANTIRAM_11YR": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, Antiram-directional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_NOSP_ANTIRAM_1YR": "IBEX-Hi Release 16; no Compton-Getting, no Survival-Probability, ANTIRAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_NOSP_OMNI_11YR": "IBEX-Hi Release 16; no Compton-Getting, no Survival-Probability, Omnidirectional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_NOSP_OMNI_6MO": "IBEX-Hi Release 16; no Compton-Getting, no Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_NOSP_RAM_11YR": "IBEX-Hi Release 16; Compton-Getting, no Survival-Probability, Ram-directional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_NOSP_RAM_1YR": "IBEX-Hi Release 16; no Compton-Getting, no Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_SP_ANTIRAM_11YR": "IBEX-Hi Release 16; no Compton-Getting, Survival-Probability, Antiram-directional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_SP_OMNI_11YR": "IBEX-Hi Release 16; no Compton-Getting, Survival-Probability, Omnidirectional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_SP_OMNI_6MO": "IBEX-Hi Release 16; no Compton-Getting, Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_SP_RAM_11YR": "IBEX-Hi Release 16; no Compton-Getting, Survival-Probability, Ram-directional 11-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_SP_RAM_1YR": "IBEX-Hi Release 16; no Compton-Getting, Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_SP_RAM_EQUA_11YR": "IBEX-Hi Release 16; no Compton-Getting, Survival-Probability, Ram-directional 11-year-Average West Ecliptic Maps in Equatorial coordinates - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_HI_R16_NOCG_SP_RAM_GALA_11YR": "IBEX-Hi Release 16; no Compton-Getting, Survival-Probability, Ram-directional 11-year-Average West Maps in Galactic coordinates - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R07_NOCG_NOSP_OMNI_6MO": "IBEX-Lo Release-07; no Compton-Getting, no Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R07_NOCG_NOSP_OMNI_VESCF_10MP": "IBEX-Lo Release 7; no Compton-Getting, no Survival-Probability, Omnidirectional 1-to-10-map Average West Ecliptic Maps in Var Energy SC Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R07_NOCG_SP_OMNI_6MO": "IBEX-Lo Release-07; no Compton-Getting, Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R07_NOCG_SP_OMNI_VESCF_10MP": "IBEX-Lo Release 7; no Compton-Getting, Survival-Probability, Omnidirectional 1-to-10-map Average West Ecliptic Maps in Var Energy SC Frame - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R08_OMNI_F2-RIBBON-MAPS-GAL_5YR": "IBEX-Lo Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R08_OMNI_F2-RIBBON-MAPS-J2000_5YR": "IBEX-Lo Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R08_OMNI_F2-RIBBON-MAPS_5YR": "IBEX-Lo Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R08_OMNI_F3-GDF-MAPS-GALACTIC_5YR": "IBEX-Lo Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R08_OMNI_F3-GDF-MAPS-J2000_5YR": "IBEX-Lo Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R08_OMNI_F3-GDF-MAPS_5YR": "IBEX-Lo Release-08; omni-direction 5-year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R09_PARK_OMAP_3YR": "IBEX-Lo Release-09; Park et al. 2015) 3-year combined heavy neutral  maps: m1-to-m6 (map1 + map2 + map3 + map4 + map5 + map6) West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R09_PARK_OMAP_3YR-EVEN-MAPS": "IBEX-Lo Release-09; Park et al. 2015) 3-year combined heavy neutral even maps: m2m4m6 (map2 + map4 + map6) West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R09_PARK_OMAP_3YR-ODD-MAPS": "IBEX-Lo Release-09; Park et al. 2015) 3-year combined heavy neutral odd maps: m1m3m5 (map1 + map3 + map5) West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R09_PARK_OMAP_6MO": "IBEX-Lo Release-09; Park Oxygen Map Counting Rate 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R09_PARK_OMAP_STAT_3YR": "IBEX-Lo Release-09; Park et al. 2015) 3-year combined heavy neutral maps: m1-to-m6 (map1 + map2 + map3 + map4 + map5 + map6) with statistical filtering - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R10_NOCG_NOSP_OMNI_6MO": "IBEX-Lo Release-10; no Compton-Getting, no Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R10_NOCG_NOSP_OMNI_7YR": "IBEX-Lo Release-10; no Compton-Getting, no Survival-Probability, Omnidirectional 7-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R10_NOCG_SP_OMNI_6MO": "IBEX-Lo Release-10; no Compton-Getting, Survival-Probability, Omnidirectional 6-month-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
     "IBEX_H3_ENA_LO_R10_NOCG_SP_OMNI_7YR": "IBEX-Lo Release-10; no Compton-Getting, Survival-Probability, Omnidirectional 7-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R11_SCHWADRON-INTERSTELLAR-O": "IBEX Release-11; Oxygen count rates for different spin phase bins organized by orbit - David McComas (Southwest Research Institute, San Antonio, TX)",
-    "IBEX_H3_ENA_LO_R17_CG_NOSP_ANTIRAM_1YR": "IBEX-lo Release 17; Compton-Getting, no Survival-Probability, ANTIRAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R17_CG_NOSP_OMNI_1YR": "IBEX-lo Release 17; Compton-Getting, no Survival-Probability, OMNIdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R17_CG_NOSP_RAM_1YR": "IBEX-lo Release 17; Compton-Getting, no Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R17_CG_SP_ANTIRAM_1YR": "IBEX-lo Release 17; Compton-Getting, Survival-Probability, ANTIRAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R17_CG_SP_OMNI_1YR": "IBEX-lo Release 17; Compton-Getting, no Survival-Probability, OMNIdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R17_CG_SP_RAM_1YR": "IBEX-lo Release 17; Compton-Getting, Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_H3_ENA_LO_R17_NOCG_NOSP_RAM_1YR": "IBEX-lo Release 17; no Compton-Getting, no Survival-Probability, RAMdirectional 1-Year-Average West Ecliptic Maps - Dr. David J. McComas (Princeton University)",
-    "IBEX_OR_SSC": "Orbit parameters from SSCWeb - SSCWeb (SPDF/Goddard)",
-    "ICON_L2-1_MIGHTI-A_LOS-WIND-GREEN": "Michelson Interferometer for Global High-resolution Thermospheric Imaging (MIGHTI) Sensor A: Line-of-sight Wind Profiles - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-1_MIGHTI-A_LOS-WIND-RED": "Michelson Interferometer for Global High-resolution Thermospheric Imaging (MIGHTI) Sensor A: Line-of-sight Wind Profiles - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-1_MIGHTI-B_LOS-WIND-GREEN": "Michelson Interferometer for Global High-resolution Thermospheric Imaging (MIGHTI) Sensor B - Line-of-sight Wind Profiles - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-1_MIGHTI-B_LOS-WIND-RED": "Michelson Interferometer for Global High-resolution Thermospheric Imaging (MIGHTI) Sensor B - Line-of-sight Wind Profiles - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-2_MIGHTI_VECTOR-WIND-GREEN": "MIGHTI - Cardinal Vector Winds - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-2_MIGHTI_VECTOR-WIND-RED": "MIGHTI - Cardinal Vector Winds - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-3_MIGHTI-A_TEMPERATURE": "ICON MIGHTI-A Level 2.3 Retrieved Temperature File - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-3_MIGHTI-B_TEMPERATURE": "ICON MIGHTI-B Level 2.3 Retrieved Temperature File - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-4_FUV_DAY": "ICON FUV Daytime: column density ratio of thermospheric atomic oxygen to molecular nitrogen.  - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-5_FUV_NIGHT": "FUV Short Wavelength Channel - 135.6 Altitude Profiles (night) - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-6_EUV": "ICON EUV derived ionospheric data products - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-7_IVM-A": "ICON Ion Velocity Meter (IVM) Thermal Plasma Measurements - T. J. Immel (UC Berkeley>SSL)",
-    "ICON_L2-7_IVM-B": "ICON IVM Thermal Plasma Measurements B - T. J. Immel (UC Berkeley>SSL)",
+    "ICON_L2-2_MIGHTI_VECTOR-WIND-GREEN": "MIGHTI - Cardinal Vector Winds - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-2_MIGHTI_VECTOR-WIND-RED": "MIGHTI - Cardinal Vector Winds - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-3_MIGHTI-A_TEMPERATURE": "ICON MIGHTI-A Level 2.3 Retrieved Temperature File - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-3_MIGHTI-B_TEMPERATURE": "ICON MIGHTI-B Level 2.3 Retrieved Temperature File - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-4_FUV_DAY": "ICON FUV Daytime - need to add more here - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-5_FUV_NIGHT": "FUV Short Wavelength Channel - 135.6 Altitude Profiles (night) - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-6_EUV": "ICON EUV derived ionospheric data products - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-7_IVM-A": "ICON Ion Velocity Meter (IVM) Thermal Plasma Measurements - T. J. Immel (UC Berkeley > SSL)",
+    "ICON_L2-7_IVM-B": "ICON IVM Thermal Plasma Measurements B - T. J. Immel (UC Berkeley > SSL)",
     "IG_K0_PCI": "Interball Polar Cap Activity Index, Key Parameters - V.Sergeev  (Institute of physics Univ. of St.-Peterburg St.-Peterburg, Russia )",
     "IMAGE_M2_EUV": "Imager for Magnetospause-to-Aurora Global Extreme Ultraviolet Imager Modified Data 2 - R. M. Katus (Eastern Michigan University)",
     "IM_ELECTRON_DENSITY_RPI": "IMAGE RPI electron density along the spacecraft orbit, IMAGE Radio Plasma Imager (RPI) - R. E. Denton & B.W. Reinisch (Dartmouth, UMLCAR)",
     "IM_HK_ADS": "Image Attitude Determination System Housekeeping - Dr. Jim Burch (Southwest Research Institute)",
     "IM_HK_AST": "Image Autonomous Star Tracker Housekeeping - Dr. Jim Burch (Southwest Research Institute)",
     "IM_HK_COM": "Image Communication Systems Housekeeping - Dr. Jim Burch (Southwest Research Institute)",
     "IM_HK_FSW": "Image Flight Software Housekeeping - Dr. Jim Burch (Southwest Research Institute)",
@@ -958,15 +861,14 @@
     "MARS_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "MAVEN_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "MERCURY_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "MESSENGER_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "MESSENGER_MAG_RTN": "MESSENGER interplanetary magnetic field (1-second/high resolution) in RTN coordinates - Prof. Sean C. Solomon (Carnegie Institution of Washington)",
     "METOP1_POES-SEM2_FLUXES-2SEC": "POES-SEM2 2-second Particle Precipitation Data, MetOp-B (MetOp-1 before Sept2012 launch) [Important: these data have known contamination problems: please consult Rob Redmon (sem.poes@noaa.gov) for usage recommendations.]  - NGDC and SWPC (NOAA)",
     "METOP2_POES-SEM2_FLUXES-2SEC": "POES-SEM2 2-second Particle Precipitation Data, MetOp-A (MetOp-2 before Oct2006 launch) [Important: these data have known contamination problems: please consult Rob Redmon (sem.poes@noaa.gov) for usage recommendations.]  - NGDC and SWPC (NOAA)",
-    "METOP3_POES-SEM2_FLUXES-2SEC": "POES-SEM2 2-second Particle Precipitation Data, MetOp-C (MetOp-3 launched 07 November 2018) [Important: these data have known contamination problems: please consult Rob Redmon (sem.poes@noaa.gov) for usage recommendations.]  - NCEI (NOAA)",
     "MMS1_ASPOC_SRVY_L2": "Level 2 Active Spacecraft Potential Control Survey Data - K. Torkar, R. Nakamura (IWF)",
     "MMS1_DSP_FAST_L2_BPSD": "SCM Low frequency Magnetic spectral density from the FIELDS Digital Signal Processor - J. Burch, R. Ergun, O. Le Contel (SWRI, LASP, LPP)",
     "MMS1_DSP_FAST_L2_EPSD": "Low and medium frequency Electric Field spectral density from the FIELDS Digital Signal Processor - J. Burch, R. Ergun (SWRI, LASP)",
     "MMS1_DSP_SLOW_L2_BPSD": "search coil magnetometer spectral density - J. Burch, R. Ergun, O. Le Contel (SWRI, LASP, LPP)",
     "MMS1_DSP_SLOW_L2_EPSD": "electric spectral density - J. Burch, R. Ergun (SWRI, LASP)",
     "MMS1_EDI_BRST_L2_AMB": "Level 2 EDI Ambient electron flux - Roy Torbert, Hans Vaith (UNH)",
     "MMS1_EDI_BRST_L2_AMB-PM2": "Level 2 EDI Ambient electron flux - Roy Torbert, Hans Vaith (UNH)",
@@ -1297,15 +1199,15 @@
     "PO_OR_DEF": "Polar Definitive Orbit Data",
     "PO_OR_PRE": "Polar Predicted Orbit Data",
     "PO_PA_DEF": "Polar Platform Attitude Definitive data",
     "PO_VIS_EARTH-CAMERA-CALIBRATED": "Polar Visible Imaging System (VIS) Earth Camera Images at ~4 minute cadence - Louis A. Frank (The University of Iowa)",
     "PO_VIS_VISIBLE-IMAGER-CALIBRATED": "Polar Visible Imaging System (VIS) Low Res. Camera - Louis A. Frank (The University of Iowa)",
     "PSP_COHO1HR_MERGED_MAG_PLASMA": "Merged hourly magnetic field, plasma, proton fluxes, and ephermis data of PSP  - Natalia Papitashvili (NASA/GSFC)",
     "PSP_FLD_L2_AEB": "PSP FIELDS L2 Data from Antenna Electronics Board (AEB) - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
-    "PSP_FLD_L2_DFB_AC_BPF_DV12HG": "PSP FIELDS Level 2 Digital Fields Board (DFB) AC Bandpass Filter (BPF) of dV12 High Gain (HG) Channel (dV12hg) - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
+    "PSP_FLD_L2_DFB_AC_BPF_DV12HG": "PSP FIELDS Level 2 DFB AC Bandpass Filter (BPF) dV12hg - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_DFB_AC_BPF_DV34HG": "PSP FIELDS Level 2 DFB AC Bandpass Filter (BPF) dV34hg - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_DFB_AC_BPF_SCMULFHG": "PSP FIELDS Level 2 DFB AC Bandpass Filter SCMulfhg - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_DFB_AC_BPF_SCMUMFHG": "PSP FIELDS Level 2 DFB AC Bandpass Filter SCMumfhg - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_DFB_AC_SPEC_DV12HG": "PSP FIELDS Level 2 DFB AC  Spectra of dV12hg Channel - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_DFB_AC_SPEC_DV34HG": "PSP FIELDS Level 2 DFB AC Spectra of dV34 High Gain (HG) Channel (DV34HG) - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_DFB_AC_SPEC_SCMDLFHG": "PSP FIELDS Level 2 DFB AC Spectra of Search Coil Magnetometer (SCM) D Low Frequency (LF) High Gain (HG) Channel (SCMDLFHG) - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_DFB_AC_SPEC_SCMELFHG": "PSP FIELDS Level 2 DFB AC Spectra of Search Coil Magnetometer (SCM) E Low Frequency (LF) High Gain (HG) Channel (SCMELFHG) - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
@@ -1348,15 +1250,14 @@
     "PSP_FLD_L2_MAG_SC": "PSP FIELDS full cadence Fluxgate Magnetometer (MAG) data in SC coordinates - Stuart D. Bale (bale@berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_MAG_SC_1MIN": "PSP FIELDS 1 minute cadence Fluxgate Magnetometer (MAG) data in SC coordinates - Stuart D. Bale (bale@berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_MAG_SC_4_SA_PER_CYC": "PSP FIELDS 4 samples per cycle cadence Fluxgate Magnetometer (MAG) data in SC coordinates - Stuart D. Bale (bale@berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_MAG_VSO": "PSP FIELDS full cadence Fluxgate Magnetometer (MAG) data in VSO coordinates - Stuart D. Bale (bale@berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_RFS_BURST": "PSP FIELDS L2 Radio Frequency Spectrometer (RFS) Burst Data - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_RFS_HFR": "PSP FIELDS Level 2 Radio Frequency Spectrometer (RFS) High Frequency Receiver (HFR) Data - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L2_RFS_LFR": "PSP FIELDS Level 2 Radio Frequency Spectrometer (RFS) Low Frequency Receiver (LFR) Data - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
-    "PSP_FLD_L2_TDS_WF": "PSP FIELDS TDS Wave-Form Burst Science Telemetry - Stuart D. Bale (bale@berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L3_MERGED_SCAM_WF": "PSP FIELDS Level 3 Merged Search Coil and Fluxgate Magnetic Field Waveform - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L3_RFS_LFR_QTN": "PSP FIELDS Level 3 Electron Density Data from Radio Frequency Spectrometer (RFS) Low Frequency Receiver (LFR) Quasi-Thermal Noise (QTN) Spectroscopy - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_FLD_L3_SQTN_RFS_V1V2": "Parker Solar Probe FIELDS Level 3 Simplified Quasi-Thermal Noise (SQTN) data, using the Radio Frequency Spectrometer (RFS) spectra when connected to V1V2 dipole antenna - Stuart D. Bale (bale@ssl.berkeley.edu) (UC Berkeley Space Sciences Laboratory)",
     "PSP_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "PSP_ISOIS-EPIHI_L2-HET-RATES10": "Parker Solar Probe ISOIS EPI-Hi Level 2 HET 10-second Rates - David McComas (Princeton University)",
     "PSP_ISOIS-EPIHI_L2-HET-RATES300": "Parker Solar Probe ISOIS EPI-Hi Level 2 HET 5-minute Rates - David McComas (Princeton University)",
     "PSP_ISOIS-EPIHI_L2-HET-RATES3600": "Parker Solar Probe ISOIS EPI-Hi Level 2 HET Hourly Rates - David McComas (Princeton University)",
@@ -1382,15 +1283,15 @@
     "PSP_SWP_SPB_SF1_L2_32E": "Electron Differential Energy Flux at each measured energy step, and averaged over all deflection steps and anodes of the SPAN-Electron instrument - J. Kasper (Univ. of Michigan)",
     "PSP_SWP_SPC_L2I": "Parker Solar Probe/SWEAP/SPC Level 2 charge flux distributions - Justin C. Kasper (University of Michigan)",
     "PSP_SWP_SPC_L3I": "Parker Solar Probe/SWEAP/SPC level 3 ion data - Justin C. Kasper (University of Michigan)",
     "PSP_SWP_SPE_SF0_L3_PAD": "Electron Pitch Angle Distribution for the SPAN-Electron instrument - J. Kasper (Univ. of Michigan)",
     "PSP_SWP_SPI_SF00_L2_8DX32EX8A": "Proton Differential Energy Flux at each measured energy/deflector step and anode of the SPAN-Ion instrument - J. Kasper (Univ. of Michigan)",
     "PSP_SWP_SPI_SF00_L3_MOM": "Partial moments of the Proton distribution function in the SPAN-Ion instrument, PSP spacecraft, and RTN coordinate systems. User should be aware that the full ion distribution is typically NOT in the FOV of the instrument. - J. Kasper (Univ. of Michigan)",
     "PSP_SWP_SPI_SF00_L3_MOM_INST": "Partial moments of the Proton distribution function in the instrument frame of reference. User should be aware that the full ion distribution is typically NOT in the FOV of the instrument. - J. Kasper (Univ. of Michigan)",
-    "PSP_SWP_SPI_SF01_L2_8DX32EX8A": "Proton-Contaminated Alpha Differential Energy Flux at Each Measured Energy/Deflector Step and Anode of the SPAN-Ion Instrument - J. Kasper (Univ. of Michigan)",
+    "PSP_SWP_SPI_SF01_L2_8DX32EX8A": "Proton-Contaminated Alpha Differential Energy Flux at Each Measured Deflector Step, Energy, and Anode from the SPAN-Ion Instrument - J. Kasper (Univ. of Michigan)",
     "PSP_SWP_SPI_SF0A_L3_MOM": "Partial moments of the Alpha distribution function in the SPAN-Ion instrument, PSP spacecraft, and RTN coordinate systems. User should be aware that the full ion distribution is typically NOT in the FOV of the instrument. - J. Kasper (Univ. of Michigan)",
     "PSP_SWP_SPI_SF0A_L3_MOM_INST": "Partial moments of the Alpha distribution function in the instrument frame of reference. User should be aware that the full ion distribution is typically NOT in the FOV of the instrument. - J. Kasper (Univ. of Michigan)",
     "RBSP-A-RBSPICE_LEV-2_ESRHELT": "High-energy low-time resolution electron fluxes ~0.02-1.0 MeV (with multi-spin accumulations plotted at end of accumulation in sector order) - Lou Lanzerotti (New Jersey Institute of Technology)",
     "RBSP-A-RBSPICE_LEV-2_ESRLEHT": "Low-energy high-time resolution electron fluxes ~0.02-1.0 MeV (with spin accumulations plotted at end of accumulation in sector order) - Lou Lanzerotti (New Jersey Institute of Technology)",
     "RBSP-A-RBSPICE_LEV-2_ISRHELT": "Diagnostic Data Use only - DO NOT USE FOR SCIENTIFIC PURPOSES. High-energy low-time resolution RBSPICE Ion Energy mode measurement of all particle fluxes (electron/ion)  ~0.05-1.0 MeV (with multi-spin accumulations plotted at end of accumulation in sector order) - Lou Lanzerotti (New Jersey Institute of Technology)",
     "RBSP-A-RBSPICE_LEV-2_TOFXEH": "TOF x Energy Hydrogen Rates (with spin accumulations plotted at end of accumulation in sector order) - Lou Lanzerotti (New Jersey Institute of Technology)",
     "RBSP-A-RBSPICE_LEV-2_TOFXEION": "TOF x Energy Ion Fluxes 0.02-1 MeV measured at high energy resolution and low time resolution  (with multi-spin accumulations plotted at end of accumulation in sector order) - Lou Lanzerotti (New Jersey Institute of Technology)",
@@ -1499,14 +1400,15 @@
     "RBSP-B_WFR-WAVEFORM_EMFISIS-L2": "WFR Three Axis Electric Field (EU, EV, EW) and Three Axis Magnetic field (BU, BV, BW)  waveforms as 16384 samples @ 35 kS/sec - Craig Kletzing (University of Iowa)",
     "RBSPA_EFW-L2_E-HIRES-UVW": "Reference for Spin Axis Vector in GSE - J. R. Wygant (University of Minnesota)",
     "RBSPA_EFW-L2_E-SPINFIT-MGSE": "Spinfit (10.9 sec resolution) DC Electric Field estimates in M-GSE coordinates. - J. R. Wygant (University of Minnesota)",
     "RBSPA_EFW-L2_ESVY_DESPUN": "Despun (32 Samples/sec) E-Field estimates in M-GSE coords - J. R. Wygant (University of Minnesota)",
     "RBSPA_EFW-L2_FBK": "Filterbank peak and average values 1-7000 Hz from RBSP-EFW (with peak and average values returned for 2 of 20 possible sources at any one time) - J. R. Wygant (University of Minnesota)",
     "RBSPA_EFW-L2_SPEC": "On-Board Spin-Fit 4-8000 Hz electric and magnetic field spectral data from RBSP-EFW (with 7 of 75 possible sources returned at any one time) - J. R. Wygant (University of Minnesota)",
     "RBSPA_EFW-L2_VSVY-HIRES": "DERIVED FROM: Spinfit DC Electric Field estimates in M-GSE coordinates - J. R. Wygant (University of Minnesota)",
+    "RBSPA_EFW-L3": "DERIVED FROM: Spinfit DC Electric Field estimates in M-GSE coordinates - J. R. Wygant (University of Minnesota)",
     "RBSPA_EFW_BURST-WAVEFORM-UVW-L1": "Burst Mode 1 (512 samples/sec) Electric and Magnetic Fields - J. R. Wygant",
     "RBSPA_L2-1MIN_PSBR-RPS": "Van Allen Probes/RPS Level 2 1-Minute Data - J. Mazur (The Aerospace Corporation)",
     "RBSPA_L2_PSBR-RPS": "Van Allen Probes/RPS Level 2 Data - J. Mazur (The Aerospace Corporation)",
     "RBSPA_REL03_ECT-MAGEIS-L2": "Electron fluxes ~20-4000 keV and proton fluxes ~50-1500 keV from ECT/MAGEIS - J. Bernard Blake / JBernard.Blake@aero.org (The Aerospace Corporation)",
     "RBSPA_REL03_ECT-REPT-SCI-L2": "Electron fluxes 2-20 MeV and proton fluxes 20-120 MeV from ECT/REPT - D. Baker (University of Colorado at Boulder)",
     "RBSPA_REL03_ECT-REPT-SCI-L3": "RBSP/ECT REPT Pitch Angle Resolved Electron and Proton Fluxes. Electron energies: 2 - 59.45 MeV. Proton energies: 21.25 - 0 MeV - D. Baker (University of Colorado at Boulder)",
     "RBSPA_REL04_ECT-HOPE-MOM-L3": "Spin resolved HOPE science data.  Plasma moments from electrons >200 eV and ions >30 eV measured at apogee in alternate spin cadence. - Herbert Funsten (Los Alamos National Laboratory)",
@@ -1516,14 +1418,15 @@
     "RBSPA_REL04_ECT-MAGEIS-L3": "Electron fluxes ~20-4000keV and proton fluxes ~60-1500 keV from ECT/MagEIS - J. Bernard Blake (JBernard.Blake@aero.org) (The Aerospace Corporation)",
     "RBSPB_EFW-L2_E-HIRES-UVW": "Reference for Spin Axis Vector in GSE - J. R. Wygant (University of Minnesota)",
     "RBSPB_EFW-L2_E-SPINFIT-MGSE": "Spinfit (10.9 sec resolution) DC Electric Field estimates in M-GSE coordinates. - J. R. Wygant (University of Minnesota)",
     "RBSPB_EFW-L2_ESVY_DESPUN": "Despun (32 Samples/sec) E-Field estimates in M-GSE coords - J. R. Wygant (University of Minnesota)",
     "RBSPB_EFW-L2_FBK": "Filterbank peak and average values 1-7000 Hz from RBSP-EFW (with peak and average values returned for 2 of 20 possible sources at any one time) - J. R. Wygant (University of Minnesota)",
     "RBSPB_EFW-L2_SPEC": "On-Board Spin-Fit 4-8000 Hz electric and magnetic field spectral data from RBSP-EFW (with 7 of 75 possible sources returned at any one time) - J. R. Wygant (University of Minnesota)",
     "RBSPB_EFW-L2_VSVY-HIRES": "DERIVED FROM: Spinfit DC Electric Field estimates in M-GSE coordinates - J. R. Wygant (University of Minnesota)",
+    "RBSPB_EFW-L3": "DERIVED FROM: Spinfit DC Electric Field estimates in M-GSE coordinates - J. R. Wygant (University of Minnesota)",
     "RBSPB_EFW_BURST-WAVEFORM-UVW-L1": "Burst Mode 1 (512 samples/sec) Electric and Magnetic Fields - J. R. Wygant",
     "RBSPB_L2-1MIN_PSBR-RPS": "Van Allen Probes/RPS Level 2 1-Minute Data - J. Mazur (The Aerospace Corporation)",
     "RBSPB_L2_PSBR-RPS": "Van Allen Probes/RPS Level 2 Data - J. Mazur (The Aerospace Corporation)",
     "RBSPB_REL03_ECT-MAGEIS-L2": "Electron fluxes ~20-4000 keV and proton fluxes ~50-1500 keV from ECT/MAGEIS - J. Bernard Blake / JBernard.Blake@aero.org (The Aerospace Corporation)",
     "RBSPB_REL03_ECT-REPT-SCI-L2": "Electron fluxes 2-20 MeV and proton fluxes 20-120 MeV from ECT/REPT - D. Baker (University of Colorado at Boulder)",
     "RBSPB_REL03_ECT-REPT-SCI-L3": "RBSP/ECT REPT Pitch Angle Resolved Electron and Proton Fluxes. Electron energies: 2 - 59.45 MeV. Proton energies: 21.25 - 0 MeV - D. Baker (University of Colorado at Boulder)",
     "RBSPB_REL04_ECT-HOPE-MOM-L3": "Spin resolved HOPE science data.  Plasma moments from electrons >200 eV and ions >30 eV measured at apogee in alternate spin cadence. - Herbert Funsten (Los Alamos National Laboratory)",
@@ -1621,14 +1524,15 @@
     "SOLO_L2_RPW-LFR-SURV-CWF-B": "Solar Orbiter Radio and Plasma Waves, Level 2 Low Frequency Receiver (LFR) Continuous Magnetic Waveform (CWF-B) in Survey Mode - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
     "SOLO_L2_RPW-LFR-SURV-CWF-E": "Solar Orbiter Radio and Plasma Waves, Level 2 Low Frequency Reciver (LFR) Continuous Electric Waveform (CWF-E) in Survey Mode - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
     "SOLO_L2_RPW-TDS-SURV-HIST1D": "Solar Orbiter Radio/Plasma Wave, TDS L2 parameters - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
     "SOLO_L2_RPW-TDS-SURV-HIST2D": "Solar Orbiter Radio/Plasma Wave, TDS L2 parameters - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
     "SOLO_L2_RPW-TDS-SURV-STAT": "Solar Orbiter Radio/Plasma Wave, TDS L2R parameters - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
     "SOLO_L2_SWA-EAS-PAD-DEF": "Solar Orbiter Level 2 Differential Energy Flux (DEF) of Pitch Angle Data (PAD) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS-PAD-DNF": "Solar Orbiter Level 2 Differential Number Flux (DNF) of Pitch Angle Data (PAD) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) - C. J. Owen (MSSL-UCL, University College London, UK)",
+    "SOLO_L2_SWA-EAS-PAD-PSD": "Solar Orbiter Level 2 Phase Space Density (PSD) of Pitch Angle Data (PAD) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS1-NM3D-DEF": "Solar Orbiter Level 2 Nominal Mode 3D Differential Energy Flux (NM3D-DEF) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 1 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS1-NM3D-DNF": "Solar Orbiter Level 2 Nominal Mode 3D Differential Number Flux (NM3D-DNF) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 1 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS1-NM3D-PSD": "Solar Orbiter Level 2 Nominal Mode 3D Phase Space Density (NM3D-PSD) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 1 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS1-SS-DEF": "Solar Orbiter Level 2 Single Strahl (SS) Differential Energy Flux (DEF) of Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 1 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS1-SS-DNF": "Solar Orbiter Level 2 Single Strahl (SS) Differential Number Flux (DNF) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 1 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS1-SS-PSD": "Solar Orbiter Level 2 Single Strahl (SS) Phase Space Density (PSD) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 1 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS2-NM3D-DEF": "Solar Orbiter Level 2 Nominal Mode 3D Differential Energy Flux (NM3D-DEF) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 2 - C. J. Owen (MSSL-UCL, University College London, UK)",
@@ -1636,21 +1540,14 @@
     "SOLO_L2_SWA-EAS2-NM3D-PSD": "Solar Orbiter Level 2 Nominal Mode 3D Phase Space Density (NM3D-PSD) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 2 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS2-SS-DEF": "Solar Orbiter Level 2 Single Strahl (SS) Differential Energy Flux (DEF) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 2 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS2-SS-DNF": "Solar Orbiter Level 2 Single Strahl (SS) Differential Number Flux (DNF) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 2 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-EAS2-SS-PSD": "Solar Orbiter Level 2 Single Strahl (SS) Phase Space Density (PSD) from Solar Wind Analyser (SWA) Electron Analyser System (EAS) Sensor 2 - C. J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-PAS-EFLUX": "Solar Orbiter Level 2 Energy Flux from Solar Wind Analyser (SWA) Proton-Alpha Sensor (PAS) - C.J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-PAS-GRND-MOM": "Solar Orbiter Level 2 Ground Calculated Moments Data from Solar Wind Analyser (SWA) Proton-Alpha Sensor (PAS)  - C.J. Owen (MSSL-UCL, University College London, UK)",
     "SOLO_L2_SWA-PAS-VDF": "Solar Orbiter Level 2 Phase Spase Distribution Function from Solar Wind Analyser (SWA) Proton-Alpha Sensor (PAS) - C.J. Owen (MSSL-UCL, University College London, UK)",
-    "SOLO_L3_RPW-BIA-DENSITY": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
-    "SOLO_L3_RPW-BIA-DENSITY-10-SECONDS": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential, downsampled - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
-    "SOLO_L3_RPW-BIA-EFIELD": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
-    "SOLO_L3_RPW-BIA-EFIELD-10-SECONDS": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector, downsampled - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
-    "SOLO_L3_RPW-BIA-SCPOT": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
-    "SOLO_L3_RPW-BIA-SCPOT-10-SECONDS": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential, downsampled - M.Maksimovic (LESIA, Observatoire de Paris-CNRS)",
-    "SOLO_L3_SWA-HIS-COMP-10MIN": "Solar Orbiter, Level 3 Data, Solar Wind Analyser, Heavy Ion Sensor Composition 10 Minute Resolution - S. Livi (SWRI)",
     "SOLO_LL02_EPD-EPT-ASUN-RATES": "Solar Orbiter Level 2 Low Latency Data from Energetic Particle Detector (EPD), Electron Proton Telescope (EPT), Anti-Sunward Direction Particle Rates - J. Rodriguez-Pacheco (Space Research Group, Universidad de Alcala)",
     "SOLO_LL02_EPD-EPT-NORTH-RATES": "Solar Orbiter Level 2 Low Latency Data from Energetic Particle Detector (EPD) Electron Proton Telescope (EPT), North Direction Particle Rates - J. Rodriguez-Pacheco (Space Research Group, Universidad de Alcala)",
     "SOLO_LL02_EPD-EPT-SOUTH-RATES": "Solar Orbiter Level 2 Low Latency Data from Energetic Particle Detector (EPD) Electron Proton Telescope (EPT), South Direction Particle Rates - J. Rodriguez-Pacheco (Space Research Group, Universidad de Alcala)",
     "SOLO_LL02_EPD-EPT-SUN-RATES": "Solar Orbiter Level 2 Low Latency Data from Energetic Particle Detector (EPD) Electron Proton Telescope (EPT) Sunward Direction Particle Rates - J. Rodriguez-Pacheco (Space Research Group, Universidad de Alcala)",
     "SOLO_LL02_EPD-HET-ASUN-RATES": "Solar Orbiter Level 2 Low Latency Data of Energetic Particle Detector (EPD) High Energy Telescope (HET) Anti-Sunward Direction Particle Rates - J. Rodriguez-Pacheco (Space Research Group, Universidad de Alcala)",
     "SOLO_LL02_EPD-HET-NORTH-RATES": "Solar Orbiter Level 2 Low Latency Data of Energetic Particle Detector (EPD) High Energy Telescope (HET) North Direction Particle Rates - J. Rodriguez-Pacheco (Space Research Group, Universidad de Alcala)",
     "SOLO_LL02_EPD-HET-SOUTH-RATES": "Solar Orbiter Level 2 Low Latency Data of Energetic Particle Detector (EPD) High Energy Telescope (HET) South Direction Particle Rates - J. Rodriguez-Pacheco (Space Research Group, Universidad de Alcala)",
@@ -1697,16 +1594,14 @@
     "STA_L2_PLA_IRON_Q_2HR": "STEREO Ahead PLASTIC Level 2  - Dr. Antoinette Galvin (University of New Hampshire)",
     "STA_L3_PLA_HE2PL_F_VSW_01HR": "He++ Phase Space Density (PSD) Binned by V/Vsw. - Dr. Antoinette Galvin (University of New Hampshire)",
     "STA_L3_PLA_HEPLUS_24HR": "STEREO Ahead PLASTIC Level 3 He+ Fluxes Binned by V/Vsw,  - Dr. Antoinette Galvin (University of New Hampshire)",
     "STA_L3_PLA_HEPLUS_F_VSW_01HR": "STEREO Ahead PLASTIC Level 3 He+ Phase Space Density (PSD) Binned by V/Vsw, Hourly Resolution.  - Dr. Antoinette Galvin (University of New Hampshire)",
     "STA_L3_PLA_HEPLUS_F_VSW_10MIN": "He+ Phase Space Density (PSD) Binned by V/Vsw. - Dr. Antoinette Galvin (University of New Hampshire)",
     "STA_L3_PLA_HEPLUS_F_VSW_24HR": "STEREO Ahead PLASTIC Level 3 He+ Phase Space Density (PSD) Binned by V/Vsw - Dr. Antoinette Galvin (University of New Hampshire)",
     "STA_L3_PLA_HEPLUS_SW_VELCTDIST_5MIN": "He+ SW Frame Velocity Count Distributions. - Dr. Antoinette Galvin (University of New Hampshire)",
-    "STA_L3_WAV_HFR": "STEREO-A/WAVES/HFR Data - Milan Maksimovic (milan.maksimovic@obspm.fr) and Stuart D. Bale (bale@berkeley.edu) (LESIA, Observatoire de Paris-PSL, CNRS and UC Berkeley Space Sciences Laboratory)",
-    "STA_L3_WAV_LFR": "STEREO-A/WAVES/LFR Data - Milan Maksimovic (milan.maksimovic@obspm.fr) and Stuart D. Bale (bale@berkeley.edu) (LESIA, Observatoire de Paris-PSL, CNRS and UC Berkeley Space Sciences Laboratory)",
     "STA_LB_IMPACT": "STEREO Ahead IMPACT Beacon Data - J. Luhmann (UCB/SSL)",
     "STA_LB_MAG_RTN": "STEREO Ahead IMPACT Reprocessed Beacon MAG Magnetic Field Vectors around 2015 Solar Conjunction - J. Luhmann (UCB/SSL)",
     "STA_LB_PLA_BROWSE": "STEREO Ahead PLASTIC Beacon Proton Parameters [PRELIM] - Dr. Antoinette Galvin (University of New Hampshire)",
     "STB_COHO1HR_MERGED_MAG_PLASMA": "Merged hourly magnetic field, plasma, proton fluxes, and ephermis data - Natasha Papitashvili (NASA/GSFC)",
     "STB_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "STB_L1_HET": "STEREO Behind IMPACT/HET Level 1 Data. - J. Luhmann (UCB/SSL)",
     "STB_L1_IMPACT_BURST": "STEREO Behind IMPACT Burst Criteria. - J. Luhmann (UCB/SSL)",
@@ -1723,20 +1618,17 @@
     "STB_L1_SWEA_DIST": "STEREO Behind IMPACT/SWEA 3D Distributions. - J. Luhmann (UCB/SSL)",
     "STB_L1_SWEA_SPEC": "STEREO Behind IMPACT/SWEA Spectra - J. Luhmann (UCB/SSL)",
     "STB_L2_MAGPLASMA_1M": "STEREO Behind IMPACT/MAG Magnetic Field and PLASTIC Solar Wind Plasma Data - J. Luhmann (UCB/SSL)",
     "STB_L2_PLA_1DMAX_10MIN": "STEREO Behind PLASTIC Level 2  - Dr. Antoinette Galvin (University of New Hampshire)",
     "STB_L2_PLA_1DMAX_1HR": "STEREO Behind PLASTIC Level 2  - Dr. Antoinette Galvin (University of New Hampshire)",
     "STB_L2_PLA_1DMAX_1MIN": "STEREO Behind PLASTIC Level 2  - Dr. Antoinette Galvin (University of New Hampshire)",
     "STB_L2_PLA_IRON_Q_2HR": "STEREO Behind PLASTIC Level 2  - Dr. Antoinette Galvin (University of New Hampshire)",
-    "STB_L3_WAV_HFR": "STEREO-B/WAVES/HFR Data - Milan Maksimovic (milan.maksimovic@obspm.fr) and Stuart D. Bale (bale@berkeley.edu) (LESIA, Observatoire de Paris-PSL, CNRS and UC Berkeley Space Sciences Laboratory)",
-    "STB_L3_WAV_LFR": "STEREO-B/WAVES/LFR Data - Milan Maksimovic (milan.maksimovic@obspm.fr) and Stuart D. Bale (bale@berkeley.edu) (LESIA, Observatoire de Paris-PSL, CNRS and UC Berkeley Space Sciences Laboratory)",
     "STB_LB_IMPACT": "STEREO Behind IMPACT Beacon Data - J. Luhmann (UCB/SSL)",
     "STB_LB_PLA_BROWSE": "STEREO Behind PLASTIC Beacon Proton Parameters [PRELIM] - Dr. Antoinette Galvin (University of New Hampshire)",
     "STEREO_LEVEL2_SWAVES": "STEREO WAVES (SWAVES) Radio Intensity Spectra, both Ahead and Behind s/c - M. Kaiser (NASA/GSFC)",
-    "STEREO_WAVES_R0_GIFWALK": "Links to STEREO pre-generated daily summary plots (png, pdf and ps files) - M. Kaiser (NASA GSFC)",
     "SUISEI_HELIO1DAY_POSITION": "Position in heliocentric coordinates from SPDF Helioweb - Natalia Papitashvili (NASA/GSFC/SPDF)",
     "SX_K0_30F": "30-s averaged fluxes: 4 Instruments  - Glenn Mason  (JHU/APL )",
     "SX_K0_POF": "SAMPEX POLARCAP Averages: 4 Instruments - G.MASON  (JHU/APL )",
     "THA_L1_STATE": "Probe state file, contains position, attitude, sun pulse data - V. Angelopoulos (UCB, NASA NAS5-02099)",
     "THA_L2_EFI": "Spacecraft-collected (EFI) Electric field - V. Angelopoulos, J. Bonnell & F. Mozer (UCB, NASA NAS5-02099)",
     "THA_L2_ESA": "THEMIS-A (P5): Electrostatic Analyzer (ESA): Electron/Ion Ground-Calculated Energy Fluxes (ions: 5 eV to 25 keV) electrons: 6 eV to 30 keV) and Moments (density, velocity, pressure, and temperature). Includes FULL, REDUCED and BURST modes. FULL: high angular resolution, low (few min) time resolution. REDUCED: degraded angular resolution, high (approx. 3 sec) time resolution. BURST: high angular resolution, high time resolution; only short bursts of data. Note that angular resolution affects moments since they are obtained integrating over the mode-specific angular distribution. - V. Angelopoulos, C.W. Carlson & J. McFadden (UCB, NASA NAS5-02099)",
     "THA_L2_FBK": "Probe Electric Field Instrument and Search Coil Magnetometer Instrument, Digital Fields Board- digitally computed Filter Bank spectra and E12 peak and average in HF band. - V. Angelopoulos, J. W. Bonnell & F. S. Mozer; A. Roux and R. E. Ergun (UCB; CETP and LASP respectively, NASA NAS5-02099)",
@@ -1979,15 +1871,14 @@
     "THG_L2_MAG_WHS": "Higher latitude chain (Lat 60.7, Long 224.9), Ground-based Vector Magnetic Field at WhiteHorse YT, Canada, 1.0 sec time Resolution.  - Dr. Kanji Hayashi (Step Polar Network)",
     "THG_L2_MAG_WLPS": "Lower latitude chain (Lat 37.9, Long 284.6), Ground-based Vector Magnetic Field at Wlpsops Island, Virginia, 0.5 sec,Falcon network - Peter Chi (UCLA, USAF Academy)",
     "THG_L2_MAG_WRTH": "Lower latitude chain (Lat 43.6, Long 264.4), Ground-based Vector Magnetic Field at Worthington, MN, 0.5 sec, McMaC network, supported under NSF grant ATM-0245139 - Peter Chi (UCLA)",
     "THG_L2_MAG_YKC": "Higher latitude chain (Lat 62.5, Long 245.5), Ground-based Vector Magnetic Field at  Yellowknife, Canada, 1.0 sec, NRCan Network - David Calp (Geological Survey of Canada)",
     "THG_L2_MAG_YKNF": "Higher latitude chain (Lat 62.5, Long 245.7), Ground-based Vector Magnetic Field at Yellowknife, Canada, 0.5 sec, THEMIS GBO network - V. Angelopoulos & C. T. Russell (UCB & UCLA respectively, NASA NAS5-02099)",
     "THG_R0_ASI": "THEMIS Ground-Based All Sky Imager (ASI) Level-0 Image Data links  - V. Angelopoulos (UCB, NASA NAS5-02099)",
     "TIMED_EDP_GUVI": "Electron Density Profiles - Andrew Christensen (Aerospace)",
-    "TIMED_L1BV20_SABER": "IR Radiances in 10 channels (1.27 to 17ym) from 0 to 150 km, Version 1.07,  - James Russell III (Hampton University)",
     "TIMED_L1CDISK_GUVI": "Airglow fluxes at 5 wavelengths bands - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_1216A_MERC_MOVIES": "Airglow flux 14 day movies, at wavelength 1216A in Mercator Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_1216A_NP_MOVIES": "Airglow flux 14 day movies, at wavelength 1216 A in North Polar Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_1216A_SP_MOVIES": "Airglow flux 14 day movies, at wavelength 1216 A in South Polar Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_1304A_MERC_MOVIES": "Airglow flux 14 day movies, at wavelength 1304A in Mercator Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_1304A_NP_MOVIES": "Airglow flux 14 day movies, at wavelength 1304A in North Polar Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_1304A_SP_MOVIES": "Airglow flux 14 day movies, at wavelength 1304A in South Polar Projection - Andrew Christensen (Aerospace)",
@@ -1996,15 +1887,14 @@
     "TIMED_L1CDISK_GUVI_1356A_SP_MOVIES": "Airglow flux 14 day movies, at wavelength 1356A in South Polar Pojection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_LBH1_MERC_MOVIES": "Airglow flux 14 day movies, at wavelength LBH1 in Mercator Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_LBH1_NP_MOVIES": "Airglow flux 14 day movies, at wavelength LBH1 in North Polar Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_LBH1_SP_MOVIES": "Airglow flux 14 day movies, at wavelength LBH1 in South Polar Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_LBH2_MERC_MOVIES": "Airglow flux 14 day movies, at wavelength LBH2 in Mercator Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_LBH2_NP_MOVIES": "Airglow flux 14 day movies, at wavelength LBH2 in North Polar Projection - Andrew Christensen (Aerospace)",
     "TIMED_L1CDISK_GUVI_LBH2_SP_MOVIES": "Airglow flux 14 day movies, at wavelength LBH2 in South Polar Projection - Andrew Christensen (Aerospace)",
-    "TIMED_L2A_SABER": "O3, CO2, H2O Mixing Ratios and O, O2, OH, NO Volume Emission Rates, also NMC Neutral Temp., Density, and Pressure, Version 2.0,  - James Russell III (Hampton University)",
     "TIMED_L3A_SEE": "Solar irradiances 0.1 - 194 nm, Version 11 - Tom Woods (LASP/CU)",
     "TIMED_WINDVECTORSNCAR_TIDI": "Zonal and meridional winds at 60 to 180 km, version 0307,  - Timothy Killeen (NCAR)",
     "TOOWINDY_E_NE": "Electron density and electric field measurements during the rocket flight. - D. Hysell (Cornell University)",
     "TSS-1R_M1_CSAA": "TSS-1R, Shuttle Attitude Data IDFS format - Tony Lavoie (Marshall Space Flight Center)",
     "TSS-1R_M1_CSAB": "TSS-1R, Orbiter and Target State Vectors IDFS format - Tony Lavoie (Marshall Space Flight Center)",
     "TSS-1R_M1_CSCA": "TSS-1R, Computed OA Data Values IDFS format - Tony Lavoie (Marshall Space Flight Center)",
     "TSS-1R_M1_CSCB": "TSS-1R, Special Computation Events IDFS format - Tony Lavoie (Marshall Space Flight Center)",
@@ -2313,17 +2203,15 @@
     "WI_EPACT_STEP-DIRECTIONAL-DIFF-HE-FLUX-10MIN": "Wind EPACT-STEP HE - Mihir Desai (University of Texas, San Antonio)",
     "WI_H0_MFI": "Wind Magnetic Fields Investigation: 3 sec, 1 min, and hourly Definitive Data. - A. Koval (UMBC, NASA/GSFC)",
     "WI_H0_SWE": "Wind SWE (Solar Wind Experiment), 6 - 12 sec Solar Wind Electron Moments - K. Ogilvie (GSFC Code 692)",
     "WI_H0_WAV": "Wind Radio/Plasma Wave, (WAVES) High Res. Plasma Density - M. L. Kaiser (GSFC)",
     "WI_H1_SWE": "Wind Solar Wind Experiment, 92-sec Solar Wind Alpha and Proton Anisotropy Analysis - K. Ogilvie (NASA GSFC)",
     "WI_H1_WAV": "Wind Radio/Plasma Wave, (WAVES) Hi-Res Parameters - M. L. Kaiser (GSFC)",
     "WI_H2_MFI": "Wind Magnetic Fields Investigation, High-resolution Definitive Data - A. Koval (UMBC, NASA/GSFC)",
-    "WI_H3-RTN_MFI": "Wind Magnetic Fields Investigation: 3 sec, 1 min, and hourly Definitive Data (RTN). - A. Koval (UMBC, NASA/GSFC)",
     "WI_H3_SWE": "Wind Solar Wind Experiment (SWE), 9 sec solar wind electron pitch-angle distributions at 12 sec cadence - K. Ogilvie (NASA/GSFC)",
-    "WI_H4-RTN_MFI": "Wind Magnetic Fields Investigation, High-resolution Definitive Data (RTN) - A. Koval (UMBC, NASA/GSFC)",
     "WI_H4_SWE": "Wind Solar Wind Experiment (SWE), 3 sec solar wind electron pitch-angle distributions at 6-12 sec cadence - K. Ogilvie (NASA/GSFC)",
     "WI_H5_SWE": "Wind Solar Wind Experiment (SWE), 9 sec solar wind electron moments at 12 sec cadence - K. Ogilvie (NASA/GSFC)",
     "WI_K0_3DP": "Wind 3-D Plasma Analyzer, Key Parameters - R. Lin/S. Bale (UC Berkeley)",
     "WI_K0_EPA": "Wind Energetic Particle Acceleration Composition Transport, Key Parameters - T. Von Roseavinge (NASA/GSFC)",
     "WI_K0_GIFWALK": "Links to Wind KP pre-generated survey and other plots - Polar-Wind-Geotail Ground System (NASA GSFC)",
     "WI_K0_MFI": "Wind Magnetic Fields Investigation, Key Parameters - R. Lepping (NASA/GSFC)",
     "WI_K0_SMS": "Solar Wind and Suprathermal Ion Composition  Instrument, Key Parameters - G. Gloeckler (U of Maryland)",
```

### Comparing `sunpy-4.1.5/sunpy/net/cdaweb/helpers.py` & `sunpy-4.1rc1/sunpy/net/cdaweb/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     --------
     >>> from sunpy.net.cdaweb import get_observatory_groups
     >>>
     >>> groups = get_observatory_groups() #doctest: +REMOTE_DATA
     >>> groups['Group'] #doctest: +REMOTE_DATA
         <Column name='Group' dtype='str55' length=...>
                         ACE
-                        AIM
                       AMPTE
         ...
                     Voyager
                        Wind
     >>> groups.loc['STEREO'] #doctest: +REMOTE_DATA
     <Row index=...>
     Group                                  Observatories
```

### Comparing `sunpy-4.1.5/sunpy/net/cdaweb/test/test_cdaweb.py` & `sunpy-4.1rc1/sunpy/net/cdaweb/test/test_cdaweb.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/cdaweb/walker.py` & `sunpy-4.1rc1/sunpy/net/cdaweb/walker.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/__init__.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/client.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/client.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/eve.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/eve.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/fermi_gbm.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/goes.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/goes.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,78 +17,78 @@
 TIME_FORMAT = config.get("general", "time_format")
 
 __all__ = ["XRSClient", "SUVIClient"]
 
 
 class XRSClient(GenericClient):
     """
-    Provides access to several GOES XRS files archive.
+    Provides access to the GOES XRS fits files archive.
 
-    For older GOES satellites (7 and below), NASA servers are used.
-    For newer GOES satellites (8 and above), NOAA servers are used.
+    Searches for GOES XRS data both on NASA servers prior to re-processed
+    GOES 13, 14 and 15 and on the NOAA archive for > GOES 13.
+    For satellite numbers > 13 the XRSClient searches the NOAA archive, and
+    returns the re-processed science-quality data for GOES 13, 14 and 15, and
+    also the new GOES-R series 16 and 17.
 
-    For GOES 8-15, the data is the re-processed science-quality data.
+    Note - the new science quality data have scaling factors removed for 13, 14 and 15
+    and they are not added to GOES 16 AND 17. This means the peak flux will be different to
+    the older version of the data, such as those collected from the NASA servers.
 
-    .. note::
+    See the following readmes about the data
 
-        The new science quality data have the scaling factors removed for GOES 8-15
-        and they are not added to GOES 16 AND 17 data products.
-        This means the peak flux will be different to the older version of the data,
-        such as those collected from the NASA servers.
+    * Reprocessed 13, 14, 15 :
+        https://satdat.ngdc.noaa.gov/sem/goes/data/science/xrs/GOES_13-15_XRS_Science-Quality_Data_Readme.pdf
 
-    See the following readmes about these data:
-
-    * GOES 1 - 7: https://umbra.nascom.nasa.gov/goes/fits/goes_fits_files_notes.txt
-
-    * Reprocessed 8 - 15: https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/GOES_1-15_XRS_Science-Quality_Data_Readme.pdf
-
-    * GOES-R 16 - 17: https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/goes16/l1b/docs/GOES-R_EXIS_XRS_L1b_Science-Quality_Data_ReadMe.pdf
+    * GOES-R 16, 17 :
+        https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/goes16/l1b/docs/GOES-R_EXIS_XRS_L1b_Science-Quality_Data_ReadMe.pdf
 
     Examples
     --------
     >>> from sunpy.net import Fido, attrs as a
     >>> results = Fido.search(a.Time("2016/1/1", "2016/1/2"),
     ...                       a.Instrument.xrs)  #doctest: +REMOTE_DATA
     >>> results  #doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
     Results from 1 Provider:
     <BLANKLINE>
     4 Results from the XRSClient:
-    Source: <8: https://umbra.nascom.nasa.gov/goes/fits
-    8-15: https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/
-    16-17: https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/
+    Source: <13: https://umbra.nascom.nasa.gov/goes/fits
+    13, 14, 15: https://satdat.ngdc.noaa.gov/sem/goes/data/science/
+    16, 17: https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/
     <BLANKLINE>
            Start Time               End Time        Instrument ... Source Provider
     ----------------------- ----------------------- ---------- ... ------ --------
     2016-01-01 00:00:00.000 2016-01-01 23:59:59.999        XRS ...   GOES     NOAA
     2016-01-02 00:00:00.000 2016-01-02 23:59:59.999        XRS ...   GOES     NOAA
     2016-01-01 00:00:00.000 2016-01-01 23:59:59.999        XRS ...   GOES     NOAA
     2016-01-02 00:00:00.000 2016-01-02 23:59:59.999        XRS ...   GOES     NOAA
     <BLANKLINE>
     <BLANKLINE>
+
     """
-    # GOES XRS data from NASA servers up to GOES 7.
+    # GOES XRS data from NASA servers up to GOES 15.
+    # The reprocessed 13, 14, 15 data should be taken from NOAA server.
     baseurl_old = r'https://umbra.nascom.nasa.gov/goes/fits/%Y/go(\d){2}(\d){6,8}\.fits'
     pattern_old = '{}/fits/{year:4d}/go{SatelliteNumber:02d}{}{month:2d}{day:2d}.fits'
-    # The reprocessed 8-15 data should be taken from NOAA.
-    baseurl_new = (r"https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/"
-                   r"goes{SatelliteNumber:02d}/gxrs-l2-irrad_science/%Y/%m/sci_gxrs-l2-irrad_g{SatelliteNumber:02d}_d%Y%m%d_.*\.nc")
+    # GOES XRS 13, 14, 15 from NOAA (re-processed data)
+    baseurl_new = (r"https://satdat.ngdc.noaa.gov/sem/goes/data/science/xrs/"
+                   r"goes{SatelliteNumber}/gxrs-l2-irrad_science/%Y/%m/sci_gxrs-l2-irrad_g{SatelliteNumber}_d%Y%m%d_.*\.nc")
     pattern_new = ("{}/goes{SatelliteNumber:02d}/gxrs-l2-irrad_science/{year:4d}/"
                    "{month:2d}/sci_gxrs-l2-irrad_g{SatelliteNumber:02d}_d{year:4d}{month:2d}{day:2d}_{}.nc")
-    # GOES-R Series 16-17 XRS data from NOAA.
+    # GOES XRS data for GOES-R Series - 16, 17
     baseurl_r = (r"https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/goes{SatelliteNumber}"
                  r"/l2/data/xrsf-l2-flx1s_science/%Y/%m/sci_xrsf-l2-flx1s_g{SatelliteNumber}_d%Y%m%d_.*\.nc")
     pattern_r = ("{}/goes/goes{SatelliteNumber:02d}/l2/data/xrsf-l2-flx1s_science/{year:4d}/"
                  "{month:2d}/sci_xrsf-l2-flx1s_g{SatelliteNumber:02d}_d{year:4d}{month:2d}{day:2d}_{}.nc")
 
     @property
     def info_url(self):
-        return ("<8: https://umbra.nascom.nasa.gov/goes/fits \n"
-                "8-15: https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/ \n"
-                "16-17: https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/")
+        return ("<13: https://umbra.nascom.nasa.gov/goes/fits \n"
+                "13, 14, 15: https://satdat.ngdc.noaa.gov/sem/goes/data/science/ \n"
+                "16, 17: https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/")
 
     def post_search_hook(self, i, matchdict):
         tr = get_timerange_from_exdict(i)
         rowdict = OrderedDict()
         rowdict['Start Time'] = tr.start
         rowdict['Start Time'].format = 'iso'
         rowdict['End Time'] = tr.end
@@ -98,23 +98,24 @@
         rowdict["Physobs"] = matchdict["Physobs"][0]
         rowdict["url"] = i["url"]
         rowdict["Source"] = matchdict["Source"][0]
         if i["url"].endswith(".fits"):
             rowdict["Provider"] = matchdict["Provider"][0]
         else:
             rowdict["Provider"] = matchdict["Provider"][1]
+
         return rowdict
 
     def search(self, *args, **kwargs):
         matchdict = self._get_match_dict(*args, **kwargs)
         # this is for the case when the timerange overlaps with the provider change.
-        if matchdict["Start Time"] < "2001-03-01" and matchdict["End Time"] >= "2001-03-01":
+        if matchdict["Start Time"] < "2009-09-01" and matchdict["End Time"] >= "2009-09-01":
             matchdict_before, matchdict_after = matchdict.copy(), matchdict.copy()
-            matchdict_after["Start Time"] = parse_time('2001-03-01')
-            matchdict_before["End Time"] = parse_time('2001-03-01')
+            matchdict_after["Start Time"] = parse_time('2009-09-01')
+            matchdict_before["End Time"] = parse_time('2009-08-31')
             metalist_before = self._get_metalist(matchdict_before)
             metalist_after = self._get_metalist(matchdict_after)
             metalist = metalist_before + metalist_after
         else:
             metalist = self._get_metalist(matchdict)
         return QueryResponse(metalist, client=self)
 
@@ -134,25 +135,25 @@
 
     def _get_metalist(self, matchdict):
         """
         Function to get the list of OrderDicts.
         This makes it easier for when searching for overlapping providers.
         """
         metalist = []
-        # The data before the re-processed GOES 8-15 data.
-        if (matchdict["End Time"] < "2001-03-01") or (matchdict["End Time"] >= "2001-03-01" and matchdict["Provider"] == ["sdac"]):
+        # the data before the re-processed GOES 13, 14, 15 data.
+        if (matchdict["End Time"] < "2009-09-01") or (matchdict["End Time"] >= "2009-09-01" and matchdict["Provider"] == ["sdac"]):
             metalist += self._get_metalist_fn(matchdict, self.baseurl_old, self.pattern_old)
-        # New data from NOAA.
+        # new data from NOAA.
         else:
             if matchdict["End Time"] >= "2017-02-07":
                 for sat in [16, 17]:
                     metalist += self._get_metalist_fn(matchdict,
                                                       self.baseurl_r.format(SatelliteNumber=sat), self.pattern_r)
             if matchdict["End Time"] <= "2020-03-04":
-                for sat in [8, 9, 10, 11, 12, 13, 14, 15]:
+                for sat in [13, 14, 15]:
                     metalist += self._get_metalist_fn(matchdict,
                                                       self.baseurl_new.format(SatelliteNumber=sat), self.pattern_new)
         return metalist
 
     @classmethod
     def _attrs_module(cls):
         return 'goes', 'sunpy.net.dataretriever.attrs.goes'
@@ -165,31 +166,37 @@
             ("GOES", "The Geostationary Operational Environmental Satellite Program."),
             ("XRS", "GOES X-ray Sensor")],
             attrs.Physobs: [('irradiance', 'the flux of radiant energy per unit area.')],
             attrs.Source: [("GOES", "The Geostationary Operational Environmental Satellite Program.")],
             attrs.Provider: [('SDAC', 'The Solar Data Analysis Center.'),
                              ('NOAA', 'The National Oceanic and Atmospheric Administration.')],
             attrs.goes.SatelliteNumber: [(str(x), f"GOES Satellite Number {x}") for x in goes_number]}
+
         return adict
 
 
 class SUVIClient(GenericClient):
     """
     Provides access to data from the GOES Solar Ultraviolet Imager (SUVI).
 
-    `SUVI data are provided by NOAA <https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/>`__.
-
-    The SUVI instrument was first included on GOES-16. It produces level 1b as
-    well as level-2 data products. Level 2 data products are a weighted average
-    of level 1b product files and therefore provide higher imaging dynamic
+    SUVI data are provided by NOAA at the following url
+    https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/
+    The SUVI instrument was first included on GOES-16. It produces level-1b as
+    well as level-2 data products. Level-2 data products are a weighted average
+    of level-1b product files and therefore provide higher imaging dynamic
     range than individual images. The exposure time of level 1b images range
-    from 1 s to 0.005 s.
-
-    SUVI supports the following wavelengths; 94, 131, 171, 195, 284, 304 angstrom.
-    If no wavelength is specified, images from all wavelengths are returned.
+    from 1 s to 0.005 s. SUVI supports the following wavelengths;
+    94, 131, 171, 195, 284, 304 angstrom. If no wavelength is specified, images
+    from all wavelengths are returned.
+
+    Note
+    ----
+    GOES-16 began providing regular level-1b data on 2018-06-01.  At the time
+    of writing, SUVI on GOES-17 is operational but currently does not provide
+    Level-2 data.
 
     Examples
     --------
     >>> from sunpy.net import Fido, attrs as a
     >>> import astropy.units as u
     >>> results = Fido.search(a.Time("2020/7/10", "2020/7/10 00:10"), a.Instrument('suvi'),a.Level.two,
     ...                       a.goes.SatelliteNumber(16), a.Wavelength(304*u.Angstrom))  #doctest: +REMOTE_DATA
@@ -204,14 +211,15 @@
                                                                ...        Angstrom
     ----------------------- ----------------------- ---------- ... ----- ----------
     2020-07-10 00:00:00.000 2020-07-10 00:04:00.000       SUVI ...     2      304.0
     2020-07-10 00:04:00.000 2020-07-10 00:08:00.000       SUVI ...     2      304.0
     2020-07-10 00:08:00.000 2020-07-10 00:12:00.000       SUVI ...     2      304.0
     <BLANKLINE>
     <BLANKLINE>
+
     """
     baseurl1b = (r'https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/goes'
                  r'{SatelliteNumber}/l1b/suvi-l1b-{elem:2}{wave:03}/%Y/%m/%d/OR_SUVI-L1b.*\.fits.gz')
     pattern1b = ('{}/goes/goes{SatelliteNumber:2d}/l{Level:2w}/suvi-l1b-{}{Wavelength:03d}/'
                  '{year:4d}/{month:2d}/{day:2d}/{}_s{:7d}{hour:2d}{minute:2d}{second:2d}'
                  '{:1d}_e{:7d}{ehour:2d}{eminute:2d}{esecond:2d}{:1d}_{}')
     baseurl2 = (r'https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/goes{SatelliteNumber}/'
@@ -221,15 +229,16 @@
                 '{eyear:4d}{emonth:2d}{eday:2d}T{ehour:2d}{eminute:2d}{esecond:2d}Z_{}')
 
     @property
     def info_url(self):
         return 'https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes'
 
     def post_search_hook(self, i, matchdict):
-        # Extracting start times and end times
+
+        # extracting start times and end times
         start = Time(datetime(i['year'], i['month'], i['day'], i['hour'], i['minute'], i['second']))
         start.format = 'iso'
         end = Time(datetime(i['year'], i['month'], i['day'], i['ehour'], i['eminute'], i['esecond']))
         end.format = 'iso'
 
         rowdict = OrderedDict()
         rowdict['Start Time'] = start
@@ -293,15 +302,15 @@
     @classmethod
     def _attrs_module(cls):
         return 'goes', 'sunpy.net.dataretriever.attrs.goes'
 
     @classmethod
     def register_values(cls):
         from sunpy.net import attrs
-        goes_number = [16, 17, 18]
+        goes_number = [16, 17]
         adict = {attrs.Instrument: [
             ("SUVI", "GOES Solar Ultraviolet Imager.")],
             attrs.goes.SatelliteNumber: [(str(x), f"GOES Satellite Number {x}") for x in goes_number],
             attrs.Source: [('GOES', 'The Geostationary Operational Environmental Satellite Program.')],
             attrs.Physobs: [('flux', 'a measure of the amount of radiation received by an object from a given source.')],
             attrs.Provider: [('NOAA', 'The National Oceanic and Atmospheric Administration.')],
             attrs.Level: [('1b', 'Solar images at six wavelengths with image exposures 10 msec or 1 sec.'),
```

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/gong.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/gong.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/lyra.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/lyra.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,38 +16,28 @@
     Examples
     --------
     >>> from sunpy.net import Fido, attrs as a
     >>> results = Fido.search(a.Time("2016/1/1", "2016/1/2"),
     ...                       a.Instrument.lyra)  #doctest: +REMOTE_DATA
     >>> results  #doctest: +REMOTE_DATA
     <sunpy.net.fido_factory.UnifiedResponse object at ...>
-    Results from 2 Providers:
+    Results from 1 Provider:
     <BLANKLINE>
     4 Results from the LYRAClient:
     Source: http://proba2.oma.be/lyra/data/bsd
     <BLANKLINE>
            Start Time               End Time        Instrument ... Provider Level
     ----------------------- ----------------------- ---------- ... -------- -----
     2016-01-01 00:00:00.000 2016-01-01 23:59:59.999       LYRA ...      ESA     2
     2016-01-01 00:00:00.000 2016-01-01 23:59:59.999       LYRA ...      ESA     3
     2016-01-02 00:00:00.000 2016-01-02 23:59:59.999       LYRA ...      ESA     2
     2016-01-02 00:00:00.000 2016-01-02 23:59:59.999       LYRA ...      ESA     3
     <BLANKLINE>
-    3 Results from the VSOClient:
-    Source: http://vso.stanford.edu/cgi-bin/search
-    Total estimated size: 2.914 Gbyte
-    <BLANKLINE>
-           Start Time               End Time        Source ... Extent Type   Size
-                                                           ...              Mibyte
-    ----------------------- ----------------------- ------ ... ----------- --------
-    2016-01-01 09:41:00.000 2016-01-01 10:40:00.000 PROBA2 ...         N/A  2328.75
-    2016-01-01 09:41:00.000 2016-01-01 10:40:00.000 PROBA2 ...         N/A 419.0625
-    2016-01-01 09:41:00.000 2016-01-01 10:40:00.000 PROBA2 ...         N/A  30.9375
-    <BLANKLINE>
     <BLANKLINE>
+
     """
     baseurl = (r'http://proba2.oma.be/lyra/data/bsd/%Y/%m/%d/'
                r'lyra_(\d){8}-000000_lev(\d){1}_std.fits')
     pattern = '{}/bsd/{year:4d}/{month:2d}/{day:2d}/{}_lev{Level:1d}_std.fits'
 
     @property
     def info_url(self):
```

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/noaa.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/noaa.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         for key in rowdict:
             if isinstance(rowdict[key], list):
                 # uses first value among the list of possible values corresponding to an Attr
                 # returned by `get_match_dict()` to be shown in query response table.
                 rowdict[key] = rowdict[key][0]
         rowdict['url'] = 'https://services.swpc.noaa.gov/json/solar-cycle/observed-solar-cycle-indices.json'
         rowdict['Instrument'] = 'NOAA-Indices'
-        # These results are not dependent on time, but we allow time as a
+        # These results are not dependant on time, but we allow time as a
         # parameter for easy searching, so remove time from the results table
         # injected by GenericClient.
         rowdict.pop('Start Time', None)
         rowdict.pop('End Time', None)
         return QueryResponse([rowdict], client=self)
 
     @classmethod
@@ -108,15 +108,15 @@
         for key in rowdict:
             if isinstance(rowdict[key], list):
                 # uses first value among the list of possible values corresponding to an Attr
                 # returned by `get_match_dict()` to be shown in query response table.
                 rowdict[key] = rowdict[key][0]
         rowdict['url'] = 'https://services.swpc.noaa.gov/json/solar-cycle/predicted-solar-cycle.json'
         rowdict['Instrument'] = 'NOAA-Predict'
-        # These results are not dependent on time, but we allow time as a
+        # These results are not dependant on time, but we allow time as a
         # parameter for easy searching, so remove time from the results table
         # injected by GenericClient.
         rowdict.pop('Start Time', None)
         rowdict.pop('End Time', None)
         return QueryResponse([rowdict], client=self)
 
     @classmethod
```

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/norh.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/norh.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/rhessi.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/rhessi.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         out : list
             Returns the urls of the observation summary file
 
         Examples
         --------
         >>> from sunpy.net.dataretriever.sources.rhessi import RHESSIClient
         >>> RHESSIClient().get_observing_summary_filename(('2011/04/04', '2011/04/04'))   # doctest: +REMOTE_DATA
-        ['...://.../hessidata/metadata/catalog/hsi_obssumm_20110404_058.fits']
+        ['https://.../hessidata/metadata/catalog/hsi_obssumm_20110404_058.fits']
         """
         dt = TimeRange(time_range)
         # remove time from dates
         dt = TimeRange(dt.start.strftime('%Y-%m-%d'), dt.end.strftime('%Y-%m-%d'))
 
         filenames = []
```

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_eve.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_eve.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_goes_ud.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_goes_ud.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 @pytest.mark.remote_data
 @pytest.mark.parametrize(
     "timerange,url_start,url_end",
     [(Time('1995/06/03 1:00', '1995/06/05'),
       'https://umbra.nascom.nasa.gov/goes/fits/1995/go07950603.fits',
       'https://umbra.nascom.nasa.gov/goes/fits/1995/go07950605.fits'),
      (Time('2008/06/02 12:00', '2008/06/04'),
-      'https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/goes10/gxrs-l2-irrad_science/2008/06/sci_gxrs-l2-irrad_g10_d20080602_v0-0-0.nc',
-      'https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/goes10/gxrs-l2-irrad_science/2008/06/sci_gxrs-l2-irrad_g10_d20080604_v0-0-0.nc'),
+      'https://umbra.nascom.nasa.gov/goes/fits/2008/go1020080602.fits',
+      'https://umbra.nascom.nasa.gov/goes/fits/2008/go1020080604.fits'),
      (Time('2020/08/02', '2020/08/04'),
       'https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/'
-      'goes16/l2/data/xrsf-l2-flx1s_science/2020/08/sci_xrsf-l2-flx1s_g16_d20200802_v2-2-0.nc',
+      'goes16/l2/data/xrsf-l2-flx1s_science/2020/08/sci_xrsf-l2-flx1s_g16_d20200802_v2-1-0.nc',
       'https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/'
-      'goes17/l2/data/xrsf-l2-flx1s_science/2020/08/sci_xrsf-l2-flx1s_g17_d20200804_v2-2-0.nc')])
+      'goes17/l2/data/xrsf-l2-flx1s_science/2020/08/sci_xrsf-l2-flx1s_g17_d20200804_v2-1-0.nc')])
 def test_get_url_for_time_range(LCClient, timerange, url_start, url_end):
     qresponse = LCClient.search(timerange)
     urls = [i['url'] for i in qresponse]
     assert isinstance(urls, list)
     assert urls[0] == url_start
     assert urls[-1] == url_end
 
@@ -53,29 +53,31 @@
     assert urls[0] == url_start
     assert urls[-1] == url_end
 
 
 @pytest.mark.remote_data
 @pytest.mark.parametrize("timerange, url_start, url_end",
                          [(a.Time("2009/08/30 00:10", "2009/09/02"),
-                           "https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/goes10/gxrs-l2-irrad_science/2009/08/sci_gxrs-l2-irrad_g10_d20090830_v0-0-0.nc",
-                           "https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/goes14/gxrs-l2-irrad_science/2009/09/sci_gxrs-l2-irrad_g14_d20090902_v0-0-0.nc")])
+                           "https://umbra.nascom.nasa.gov/goes/fits/2009/go1020090830.fits",
+                           "https://satdat.ngdc.noaa.gov/sem/goes/data/science/xrs/goes14/gxrs-l2-irrad_science/"
+                           "2009/09/sci_gxrs-l2-irrad_g14_d20090902_v0-0-0.nc")])
 def test_get_overlap_providers(LCClient, timerange, url_start, url_end):
     qresponse = LCClient.search(timerange)
     urls = [i['url'] for i in qresponse]
-    assert len(urls) == 6
+    assert len(urls) == 4
     assert urls[0] == url_start
     assert urls[-1] == url_end
 
 
 @pytest.mark.remote_data
 @pytest.mark.parametrize("timerange, url_old, url_new",
                          [(a.Time('2013/10/28', '2013/10/29'),
                            "https://umbra.nascom.nasa.gov/goes/fits/2013/go1520131028.fits",
-                           "https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/goes13/gxrs-l2-irrad_science/2013/10/sci_gxrs-l2-irrad_g13_d20131028_v0-0-0.nc")])
+                           "https://satdat.ngdc.noaa.gov/sem/goes/data/science/xrs/goes13/gxrs-l2-irrad_science/"
+                           "2013/10/sci_gxrs-l2-irrad_g13_d20131028_v0-0-0.nc")])
 def test_old_data_access(timerange, url_old, url_new):
     # test first for old data
     qr = Fido.search(timerange, a.Instrument("XRS"), a.Provider("SDAC"))
     urls = qr[0]['url']
     assert urls[0] == url_old
 
     # now test for new data
@@ -96,24 +98,31 @@
 
 @pytest.mark.filterwarnings('ignore:ERFA function.*dubious year')
 @pytest.mark.remote_data
 def test_fixed_satellite(LCClient):
     ans1 = LCClient.search(a.Time("2017/01/01 2:00", "2017/01/02 2:10"),
                            a.Instrument.xrs,
                            a.goes.SatelliteNumber.fifteen)
+
     for resp in ans1:
+
         assert "g15" in resp['url']
+
     ans1 = LCClient.search(a.Time("2017/01/01", "2017/01/02 23:00"),
                            a.Instrument.xrs,
                            a.goes.SatelliteNumber(13))
+
     for resp in ans1:
+
         assert "g13" in resp['url']
+
     ans1 = LCClient.search(a.Time("1999/1/13", "1999/1/16"),
                            a.Instrument.xrs,
                            a.goes.SatelliteNumber(8))
+
     for resp in ans1:
         assert "go08" in resp['url']
 
 
 @pytest.mark.parametrize("time", [
     Time('2005/4/27', '2005/4/27 12:00'),
     Time('2016/2/4', '2016/2/10')])
```

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,27 +64,25 @@
     assert qr1[-1]['End Time'] == time.end + almost_day
 
 
 @pytest.mark.remote_data
 @pytest.mark.parametrize("time,instrument", [
     (Time('2013/8/27', '2013/8/27'), Instrument('lyra'))])
 def test_get(LCClient, time, instrument):
-    # Cut it down to one file with the level
-    qr1 = LCClient.search(time, instrument, a.Level.two)
+    qr1 = LCClient.search(time, instrument)
     download_list = LCClient.fetch(qr1)
     assert len(download_list) == len(qr1)
 
 
 @pytest.mark.remote_data
 @pytest.mark.parametrize(
     "time, instrument",
-    [(a.Time('2012/10/4', '2012/10/4'), a.Instrument.lyra)])
+    [(a.Time('2012/10/4', '2012/10/6'), a.Instrument.lyra)])
 def test_fido(time, instrument):
-    # Cut it down to one file with the level
-    qr = Fido.search(time, instrument, a.Level.two)
+    qr = Fido.search(time, instrument)
     assert isinstance(qr, UnifiedResponse)
     response = Fido.fetch(qr)
     assert len(response) == qr._numfile
 
 
 def test_attr_reg():
     assert a.Instrument.lyra == a.Instrument('LYRA')
```

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_noaa.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_noaa.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_norh.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_norh.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     LCClient = norh.NoRHClient()
     qr1 = LCClient.search(time, a.Instrument.norh, wave)
     assert isinstance(qr1, QueryResponse)
     # Not all hypothesis queries are going to produce results, and
     if qr1:
         # There are no observations everyday
         #  so the results found have to be equal or later than the queried time
-        #  (looking at the date because it may search for milliseconds, but only date is available)
+        #  (looking at the date because it may search for miliseconds, but only date is available)
         assert qr1[0]['Start Time'].strftime('%Y-%m-%d') >= time.start.strftime('%Y-%m-%d')
         #  and the end time equal or smaller.
         # hypothesis can give same start-end, but the query will give you from start to end (so +1)
         assert qr1[-1]['End Time'] <= time.end + TimeDelta(1*u.day)
 
 
 @pytest.mark.parametrize("time,instrument,wave", [
```

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/sources/tests/test_rhessi.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/sources/tests/test_rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/dataretriever/tests/test_client.py` & `sunpy-4.1rc1/sunpy/net/dataretriever/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/fido_factory.py` & `sunpy-4.1rc1/sunpy/net/fido_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,26 @@
 import os
 from pathlib import Path
 from textwrap import dedent
 from collections.abc import Sequence
 
 import numpy as np
 import parfive
-from packaging.version import Version
 
 from astropy.table import Table
 
 from sunpy import config
 from sunpy.net import attr, vso
 from sunpy.net.base_client import BaseClient, QueryResponseColumn, QueryResponseRow, QueryResponseTable
 from sunpy.util.datatype_factory_base import BasicRegistrationFactory, NoMatchError
 from sunpy.util.parfive_helpers import Downloader, Results
 from sunpy.util.util import get_width
 
 __all__ = ['Fido', 'UnifiedResponse', 'UnifiedDownloaderFactory']
 
-parfive_version = Version(parfive.__version__)
-
 
 class UnifiedResponse(Sequence):
     """
     The object used to store results from `~sunpy.net.fido_factory.UnifiedDownloaderFactory.search`.
 
     The `~sunpy.net.Fido` object returns results from multiple different
     clients. So it is always possible to sub-select these results, you can
@@ -380,32 +377,29 @@
         if not os.access(exists[0], os.W_OK):
             raise PermissionError('You do not have permission to write'
                                   f' to the directory {exists[0]}.')
 
         if "wait" in kwargs:
             raise ValueError("wait is not a valid keyword argument to Fido.fetch.")
 
+        # TODO: Remove when parfive allows us to special case URLS.
         # Avoid more than one connection for JSOC only requests.
         from sunpy.net.jsoc import JSOCClient
 
-        max_splits = kwargs.get('max_splits', 5)
         is_jsoc_only = False
         for query_result in query_results:
             if isinstance(query_result, UnifiedResponse):
                 is_jsoc_only = all([isinstance(result.client, JSOCClient) for result in query_result])
             elif isinstance(query_result, QueryResponseTable):
                 is_jsoc_only = all([isinstance(result.table.client, JSOCClient) for result in query_result])
         if downloader is None:
             if is_jsoc_only:
                 max_conn = 1
-                max_splits = 1
-            if parfive_version >= Version("2.0.0"):
-                downloader = Downloader(max_conn=max_conn, progress=progress, overwrite=overwrite, max_splits=max_splits)
-            else:
-                downloader = Downloader(max_conn=max_conn, progress=progress, overwrite=overwrite)
+                kwargs['max_splits'] = 1
+            downloader = Downloader(max_conn=max_conn, progress=progress, overwrite=overwrite)
         elif not isinstance(downloader, parfive.Downloader):
             raise TypeError("The downloader argument must be a parfive.Downloader instance.")
 
         # Handle retrying failed downloads
         retries = [isinstance(arg, Results) for arg in query_results]
         if all(retries):
             results = Results()
@@ -432,15 +426,16 @@
                 result = block.client.fetch(block, path=path,
                                             downloader=downloader,
                                             wait=False, **kwargs)
                 if result not in (NotImplemented, None):
                     reslist.append(result)
 
         results = downloader.download()
-        # Combine the results objects from all the clients into one Results object.
+        # Combine the results objects from all the clients into one Results
+        # object.
         for result in reslist:
             if not isinstance(result, Results):
                 raise TypeError(
                     "If wait is False a client must return a parfive.Downloader and either None"
                     " or a parfive.Results object.")
             results.data += result.data
             results._errors += result.errors
```

### Comparing `sunpy-4.1.5/sunpy/net/hek/attrs.py` & `sunpy-4.1rc1/sunpy/net/hek/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/hek/hek.py` & `sunpy-4.1rc1/sunpy/net/hek/hek.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/hek/tests/test_hek.py` & `sunpy-4.1rc1/sunpy/net/hek/tests/test_hek.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     # To check that the following bug is fixed:
     # https://github.com/sunpy/sunpy/issues/3238
     client = hek.HEKClient()
     result = client.search(attrs.Time('2013/02/01 00:00:00', '2013/02/01 23:30:00'),
                            attrs.hek.FRM.Name == 'SPoCA')
     assert isinstance(result, hek.hek.HEKTable)
     assert len(result) == 89
-    assert result[0]["SOL_standard"] == 'SOL2013-01-31T20:13:31L199C128'
+    assert result[0]["SOL_standard"] == 'SOL2013-01-31T20:13:31L219C160'
 
 
 @pytest.mark.remote_data
 def test_mixed_results_get_2():
     # To check that the following bug is fixed:
     # # https://github.com/sunpy/sunpy/issues/3898
     client = hek.HEKClient()
```

### Comparing `sunpy-4.1.5/sunpy/net/hek2vso/hek2vso.py` & `sunpy-4.1rc1/sunpy/net/hek2vso/hek2vso.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/hek2vso/tests/test_hek2vso.py` & `sunpy-4.1rc1/sunpy/net/hek2vso/tests/test_hek2vso.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/helio/chaincode.py` & `sunpy-4.1rc1/sunpy/net/helio/chaincode.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,20 +57,19 @@
         if chaincode.isdigit():
             for index, step in enumerate(chaincode):
                 self.coordinates[:, index + 1] = self.coordinates[:, index] + \
                     [[x_steps[int(step)] * xdelta,
                       y_steps[int(step)] * ydelta]]
 
     def matchend(self, end):
-        return np.all(np.equal(self.coordinates[:, -1], np.asarray(end)))
+        return np.alltrue(np.equal(self.coordinates[:, -1], np.asarray(end)))
 
     def matchany(self, coordinates, index):
-        return np.all(
-            np.allclose(self.coordinates[:, index],  np.asarray(coordinates))
-        )
+        return np.alltrue(np.allclose(self.coordinates[:, index],
+                                      np.asarray(coordinates)))
 
     def boundingbox(self):
         """
         Extract the coordinates of the chaincode.
 
         Returns in the form of ``[[x0, x1], [y0, y1]]``.
         """
```

### Comparing `sunpy-4.1.5/sunpy/net/helio/hec.py` & `sunpy-4.1rc1/sunpy/net/helio/hec.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
         Examples
         --------
         >>> from sunpy.net.helio import attrs as ha
         >>> from sunpy.net import attrs as a, Fido
         >>> timerange = a.Time('2005/01/03', '2005/12/03')
         >>> res = Fido.search(timerange, ha.MaxRecords(10),
-        ...                   ha.TableName('rhessi_hxr_flare'))  # doctest: +SKIP
-        >>> res   # doctest: +SKIP
+        ...                   ha.TableName('rhessi_hxr_flare'))  # doctest: +REMOTE_DATA
+        >>> res  #doctest: +REMOTE_DATA
         <sunpy.net.fido_factory.UnifiedResponse object at ...>
         Results from 1 Provider:
         <BLANKLINE>
         10 Results from the HECClient:
         hec_id      time_start          time_peak      ... energy_kev flare_number
         ------ ------------------- ------------------- ... ---------- ------------
          31463 2005-01-03T01:37:36 2005-01-03T01:37:54 ...          6      5010320
```

### Comparing `sunpy-4.1.5/sunpy/net/helio/parser.py` & `sunpy-4.1rc1/sunpy/net/helio/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     -------
     links: list or NoneType
         List of urls to registries containing WSDL endpoints.
 
     Examples
     --------
     >>> from sunpy.net.helio import parser
-    >>> parser.webservice_parser()  # doctest: +SKIP
+    >>> parser.webservice_parser()  # doctest: +REMOTE_DATA
     ['http://helio.mssl.ucl.ac.uk/helio-hec/HelioService',
     'http://msslkk.mssl.ucl.ac.uk/helio-hec/HelioService',
     'http://voparis-helio.obspm.fr/helio-hec/HelioService',
     'http://hec.helio-vo.eu/helio-hec/HelioService',
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioLongQueryService',
     'http://msslkk.mssl.ucl.ac.uk/helio-hec/HelioLongQueryService',
     'http://voparis-helio.obspm.fr/helio-hec/HelioLongQueryService',
@@ -90,15 +90,15 @@
     endpoints: list or NoneType
         A list containing all of the available WSDL endpoints from the passed
         in url.
 
     Examples
     --------
     >>> from sunpy.net.helio import parser
-    >>> parser.endpoint_parser('http://msslkz.mssl.ucl.ac.uk/helio-hec/HelioService')  # doctest: +SKIP
+    >>> parser.endpoint_parser('http://msslkz.mssl.ucl.ac.uk/helio-hec/HelioService')  # doctest: +REMOTE_DATA
     ['http://helio.mssl.ucl.ac.uk/helio-hec/HelioService?wsdl',
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioService1_0?wsdl',
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioService1_0b?wsdl',
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioLongQueryService?wsdl',
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioLongQueryService1_0?wsdl',
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioLongQueryService1_1?wsdl',
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioLongQueryService1_0b?wsdl',
@@ -136,15 +136,15 @@
     -------
     taverna_links: list or NoneType
         A list containing WSDL links for a taverna web-service
 
     Examples
     --------
     >>> from sunpy.net.helio import parser
-    >>> parser.taverna_parser('http://msslkz.mssl.ucl.ac.uk/helio-hec/HelioService')  # doctest: +SKIP
+    >>> parser.taverna_parser('http://msslkz.mssl.ucl.ac.uk/helio-hec/HelioService')  # doctest: +REMOTE_DATA
     ['http://helio.mssl.ucl.ac.uk/helio-hec/HelioTavernaService?wsdl']
 
     """
     endpoints = endpoint_parser(link)
     taverna_links = []
     if endpoints is None:
         return None
@@ -172,17 +172,17 @@
     -------
     webpage: str or NoneType
         String containing the webresults
 
     Examples
     --------
     >>> from sunpy.net.helio import parser
-    >>> result = parser.link_test('http://msslkz.mssl.ucl.ac.uk/helio-hec/HelioService')  # doctest: +SKIP
+    >>> result = parser.link_test('http://msslkz.mssl.ucl.ac.uk/helio-hec/HelioService')  # doctest: +REMOTE_DATA
 
-    >>> print(parser.link_test('http://rrnx.invalid_url5523.com'))  # doctest: +SKIP
+    >>> print(parser.link_test('http://rrnx.invalid_url5523.com'))  # doctest: +REMOTE_DATA
         None
     """
     try:
         with closing(urlopen(link, timeout=LINK_TIMEOUT)) as fd:
             return fd.read()
     except Exception as e:
         log.debug(f"Failed to get {link} with {e}")
@@ -208,15 +208,15 @@
     -------
     wsdl: str
         URL to a single live taverna endpoint
 
     Examples
     --------
     >>> from sunpy.net.helio import parser
-    >>> parser.wsdl_retriever()  # doctest: +SKIP
+    >>> parser.wsdl_retriever()  # doctest: +REMOTE_DATA
     'http://helio.mssl.ucl.ac.uk/helio-hec/HelioTavernaService?wsdl'
 
     Notes
     -----
     * Currently only support for HEC exists, but it was designed so that it
         could be expanded at a later date
     * There is a 3 second timeout lifespan on links, so there is potential for
```

### Comparing `sunpy-4.1.5/sunpy/net/helio/tests/test_chaincode.py` & `sunpy-4.1rc1/sunpy/net/helio/tests/test_chaincode.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/helio/tests/test_helio.py` & `sunpy-4.1rc1/sunpy/net/helio/tests/test_helio.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     taverna_parser,
     webservice_parser,
     wsdl_retriever,
 )
 
 # Currently helio makes unverified requests - this filter should be removed when
 # https://github.com/sunpy/sunpy/issues/4401 is fixed
-pytestmark = [pytest.mark.filterwarnings('ignore:Unverified HTTPS request is being made'), pytest.mark.xfail(reason="HEC is currently down")]
+pytestmark = pytest.mark.filterwarnings('ignore:Unverified HTTPS request is being made')
 
 
 def wsdl_endpoints():
     """
     Slightly simplified form of the content on http://msslkz.mssl.ucl.ac.uk/helio-hec/HelioService
     Intentionally contains duplicate URLs
     """
```

### Comparing `sunpy-4.1.5/sunpy/net/helioviewer.py` & `sunpy-4.1rc1/sunpy/net/helioviewer.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/jsoc/attrs.py` & `sunpy-4.1rc1/sunpy/net/jsoc/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/jsoc/data/attrs.json` & `sunpy-4.1rc1/sunpy/net/jsoc/data/attrs.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -2739,8 +2739,8 @@
 0000ab20: 0a20 2020 2020 2022 767a 222c 0a20 2020  .      "vz",.   
 0000ab30: 2020 2022 7261 6469 616c 2076 656c 6f63     "radial veloc
 0000ab40: 6974 7920 636f 6d70 6f6e 656e 7422 0a20  ity component". 
 0000ab50: 2020 205d 2c0a 2020 2020 5b0a 2020 2020     ],.    [.    
 0000ab60: 2020 2277 222c 0a20 2020 2020 2022 546f    "w",.      "To
 0000ab70: 7461 6c20 6f66 2031 2f6d 7520 696e 2031  tal of 1/mu in 1
 0000ab80: 2064 6567 206c 6174 6974 7564 6520 6269   deg latitude bi
-0000ab90: 6e73 220a 2020 2020 5d0a 2020 5d0a 7d    ns".    ].  ].}
+0000ab90: 6e73 220a 2020 2020 5d0a 2020 5d0a 7d0a  ns".    ].  ].}.
```

### Comparing `sunpy-4.1.5/sunpy/net/jsoc/jsoc.py` & `sunpy-4.1rc1/sunpy/net/jsoc/jsoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import time
 import urllib
 from pathlib import Path
 
 import drms
 import numpy as np
 import parfive
-from packaging.version import Version
 
 import astropy.table
 import astropy.time
 import astropy.units as u
 from astropy.utils.misc import isiterable
 
 from sunpy import config, log
@@ -23,15 +22,14 @@
 from sunpy.util.parfive_helpers import Downloader, Results
 
 __all__ = ['JSOCClient', 'JSOCResponse']
 
 
 PRIMEKEY_LIST_TIME = {'T_START', 'T_REC', 'T_OBS', 'MidTime', 'OBS_DATE',
                       'obsdate', 'DATE_OBS', 'starttime', 'stoptime', 'UTC_StartTime'}
-parfive_version = Version(parfive.__version__)
 
 
 class NotExportedError(Exception):
     pass
 
 
 class JSOCResponse(QueryResponseTable):
@@ -480,15 +478,15 @@
         """
         c = drms.Client()
 
         # Private communication from JSOC say we should not use more than one connection.
         max_splits = kwargs.get('max_splits', 1)
         if max_splits != 1:
             log.info(f"Setting max_splits to it's maximum allowed value of 1 for requests made by the JSOCClient.")
-            max_splits = 1
+        kwargs['max_splits'] = 1
 
         # Convert Responses to a list if not already
         if isinstance(requests, str) or not isiterable(requests):
             requests = [requests]
 
         # Ensure all the requests are drms ExportRequest objects
         for i, request in enumerate(requests):
@@ -530,35 +528,32 @@
 
         dl_set = True
         if not downloader:
             dl_set = False
             # Private communication from JSOC say we should not use more than one connection.
             if max_conn != self.default_max_conn:
                 log.info(f"Setting max parallel downloads to 1 for the JSOC client.")
-            if parfive_version >= Version("2.0.0"):
-                downloader = Downloader(max_conn=max_conn, progress=progress, overwrite=overwrite, max_splits=max_splits)
-            else:
-                downloader = Downloader(max_conn=max_conn, progress=progress, overwrite=overwrite)
+            downloader = Downloader(progress=progress, overwrite=overwrite, max_conn=1)
 
         urls = []
         for request in requests:
             if request.status == 0:
                 if request.protocol == 'as-is' or request.method == 'url-tar':
                     urls.extend(list(request.urls.url))
                 else:
-                    for _, data in request.data.iterrows():
+                    for index, data in request.data.iterrows():
                         url_dir = request.request_url + '/'
                         urls.append(urllib.parse.urljoin(url_dir, data['filename']))
 
         if urls:
             if progress:
                 print_message = "{0} URLs found for download. Full request totalling {1}MB"
                 print(print_message.format(len(urls), request._d['size']))
             for aurl, fname in zip(urls, paths):
-                downloader.enqueue_file(aurl, filename=fname, max_splits=max_splits)
+                downloader.enqueue_file(aurl, filename=fname)
 
         if dl_set and not wait:
             return Results()
 
         results = downloader.download()
         return results
```

### Comparing `sunpy-4.1.5/sunpy/net/jsoc/tests/test_attr.py` & `sunpy-4.1rc1/sunpy/net/jsoc/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/jsoc/tests/test_jsoc.py` & `sunpy-4.1rc1/sunpy/net/jsoc/tests/test_jsoc.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/scraper.py` & `sunpy-4.1rc1/sunpy/net/scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,22 +59,24 @@
     pattern : `str`
         A converted string with the kwargs.
     now : `datetime.datetime`
         The pattern with the actual date.
 
     Examples
     --------
+    >>> # Downloading data from SolarMonitor.org
     >>> from sunpy.net import Scraper
-    >>> pattern = ('http://proba2.oma.be/{instrument}/data/bsd/%Y/%m/%d/'
-    ...            '{instrument}_lv1_%Y%m%d_%H%M%S.fits')
-    >>> swap = Scraper(pattern, instrument='swap')
-    >>> print(swap.pattern)
-    http://proba2.oma.be/swap/data/bsd/%Y/%m/%d/swap_lv1_%Y%m%d_%H%M%S.fits
-    >>> print(swap.now)  # doctest: +SKIP
-    http://proba2.oma.be/swap/data/bsd/2022/12/21/swap_lv1_20221221_112433.fits
+    >>> solmon_pattern = ('http://solarmonitor.org/data/'
+    ...                   '%Y/%m/%d/fits/{instrument}/'
+    ...                   '{instrument}_{wave:05d}_fd_%Y%m%d_%H%M%S.fts.gz')
+    >>> solmon = Scraper(solmon_pattern, instrument = 'swap', wave = 174)
+    >>> print(solmon.pattern)
+    http://solarmonitor.org/data/%Y/%m/%d/fits/swap/swap_00174_fd_%Y%m%d_%H%M%S.fts.gz
+    >>> print(solmon.now)  # doctest: +SKIP
+    http://solarmonitor.org/data/2017/11/20/fits/swap/swap_00174_fd_20171120_193933.fts.gz
 
     Notes
     -----
     The ``now`` attribute does not return an existent file, but just how the
     pattern looks with the actual time.
     """
 
@@ -254,23 +256,25 @@
         -------
         filesurls : `list` of `str`
             List of all the files found between the time range given.
 
         Examples
         --------
         >>> from sunpy.net import Scraper
-        >>> pattern = ('http://proba2.oma.be/{instrument}/data/bsd/%Y/%m/%d/'
-        ...            '{instrument}_lv1_%Y%m%d_%H%M%S.fits')
-        >>> swap = Scraper(pattern, instrument='swap')
+        >>> solmon_pattern = ('http://solarmonitor.org/data/'
+        ...                   '%Y/%m/%d/fits/{instrument}/'
+        ...                   '{instrument}_{wave:05d}_fd_%Y%m%d_%H%M%S.fts.gz')
+        >>> solmon = Scraper(solmon_pattern, instrument = 'swap', wave = 174)
         >>> from sunpy.time import TimeRange
-        >>> timerange = TimeRange('2015-01-01T00:08:00','2015-01-01T00:12:00')
-        >>> print(swap.filelist(timerange))  # doctest: +REMOTE_DATA
-        ['http://proba2.oma.be/swap/data/bsd/2015/01/01/swap_lv1_20150101_000857.fits',
-         'http://proba2.oma.be/swap/data/bsd/2015/01/01/swap_lv1_20150101_001027.fits',
-         'http://proba2.oma.be/swap/data/bsd/2015/01/01/swap_lv1_20150101_001157.fits']
+        >>> timerange = TimeRange('2015-01-01','2015-01-01T16:00:00')
+        >>> print(solmon.filelist(timerange))  # doctest: +REMOTE_DATA
+        ['http://solarmonitor.org/data/2015/01/01/fits/swap/swap_00174_fd_20150101_025423.fts.gz',
+         'http://solarmonitor.org/data/2015/01/01/fits/swap/swap_00174_fd_20150101_061145.fts.gz',
+         'http://solarmonitor.org/data/2015/01/01/fits/swap/swap_00174_fd_20150101_093037.fts.gz',
+         'http://solarmonitor.org/data/2015/01/01/fits/swap/swap_00174_fd_20150101_124927.fts.gz']
 
         Notes
         -----
         The search is strict with the time range, so if the archive scraped contains daily files,
         but the range doesn't start from the beginning of the day, then the file for that day
         won't be selected. The end of the timerange will normally be OK as includes the file
         on such end time.
```

### Comparing `sunpy-4.1.5/sunpy/net/tests/strategies.py` & `sunpy-4.1rc1/sunpy/net/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/tests/test_attr.py` & `sunpy-4.1rc1/sunpy/net/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/tests/test_attr_walker.py` & `sunpy-4.1rc1/sunpy/net/tests/test_attr_walker.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/tests/test_baseclient.py` & `sunpy-4.1rc1/sunpy/net/tests/test_baseclient.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/tests/test_fido.py` & `sunpy-4.1rc1/sunpy/net/tests/test_fido.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,23 +176,23 @@
 UnifiedResponse Tests
 """
 
 
 @pytest.mark.remote_data
 def test_unifiedresponse_slicing():
     results = Fido.search(
-        a.Time("2012/1/1", "2012/1/2"), a.Instrument.lyra)
+        a.Time("2012/1/1", "2012/1/5"), a.Instrument.lyra)
     assert isinstance(results[0:2], UnifiedResponse)
     assert isinstance(results[0], QueryResponseTable)
 
 
 @pytest.mark.remote_data
 def test_unifiedresponse_slicing_reverse():
     results = Fido.search(
-        a.Time("2012/1/1", "2012/1/2"), a.Instrument.lyra)
+        a.Time("2012/1/1", "2012/1/5"), a.Instrument.lyra)
     assert isinstance(results[::-1], UnifiedResponse)
     assert len(results[::-1]) == len(results[::1])
     assert isinstance(results[0, ::-1], QueryResponseTable)
     assert all(results[0][::-1] == results[0, ::-1])
 
 
 @mock.patch("sunpy.net.vso.vso.build_client", return_value=True)
@@ -202,49 +202,52 @@
     uresp = UnifiedResponse(vrep)
     assert isinstance(uresp, UnifiedResponse)
 
 
 @pytest.mark.remote_data
 def test_responses():
     results = Fido.search(
-        a.Time("2012/1/1", "2012/1/2"), a.Instrument.lyra)
-    assert isinstance(results, UnifiedResponse)
-    for resp in results:
+        a.Time("2012/1/1", "2012/1/5"), a.Instrument.lyra)
+
+    for i, resp in enumerate(results):
         assert isinstance(resp, QueryResponse)
 
+    assert i + 1 == len(results)
+
 
 @pytest.mark.remote_data
 def test_repr():
     results = Fido.search(
-        a.Time("2012/1/1", "2012/1/2"), a.Instrument.lyra)
+        a.Time("2012/1/1", "2012/1/5"), a.Instrument.lyra)
+
     rep = repr(results)
     rep = rep.split('\n')
     # 8 header lines, the results table and two blank lines at the end
     assert len(rep) == 8 + len(list(results)[0]) + 2
 
 
 def filter_queries(queries):
     return attr.and_(queries) not in queries
 
 
 @pytest.mark.remote_data
-def test_path(tmp_path):
+def test_path():
     results = Fido.search(
-        a.Time("2022/1/1", "2022/1/1"), a.Instrument.aia)
-    file = Fido.fetch(results, path=tmp_path / "{file}")
-    assert file == [f'{tmp_path}/aia_lev1_335a_2022_01_01t00_00_00_62z_image_lev1.fits']
+        a.Time("2012/1/1", "2012/1/5"), a.Instrument.lyra)
+
+    Fido.fetch(results, path="notapath/{file}")
 
 
 @pytest.mark.remote_data
 @skip_windows
 def test_path_read_only(tmp_path):
     results = Fido.search(
-        a.Time("2012/1/1", "2012/1/1"), a.Instrument.lyra, a.Level.two
-    )
-    # chmod doesn't seem to work correctly on the windows CI
+        a.Time("2012/1/1", "2012/1/5"), a.Instrument.lyra)
+
+    # chmod dosen't seem to work correctly on the windows CI
     os.chmod(tmp_path, S_IREAD | S_IRGRP | S_IROTH)
     # Check to see if it's actually read only before running the test
     if not os.access(tmp_path, os.W_OK):
         with pytest.raises(PermissionError):
             Fido.fetch(results, path=tmp_path / "{file}")
```

### Comparing `sunpy-4.1.5/sunpy/net/tests/test_helioviewer.py` & `sunpy-4.1rc1/sunpy/net/tests/test_helioviewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 """
 import os
 import urllib
 from collections import OrderedDict
 
 import pytest
 
+import sunpy
+import sunpy.map
 from sunpy.net.helioviewer import HelioviewerClient
+from sunpy.tests.helpers import figure_test, skip_glymur
 
 pytestmark = pytest.mark.filterwarnings('ignore:The HelioviewerClient class is deprecated')
 
 
 @pytest.fixture(scope="function")
 def client():
     """
@@ -95,14 +98,27 @@
                                     instrument='EIT', measurement='304')
     header2 = client.get_jp2_header('1994/01/01', jp2_id=1795504)
     assert header1 == header2
     assert len(header1) == len(header2) == 1
     assert ('fits' in header1.keys()) and ('fits' in header2.keys())
 
 
+@skip_glymur
+@figure_test
+@pytest.mark.remote_data
+@pytest.mark.filterwarnings("ignore::sunpy.util.SunpyMetadataWarning")
+def test_download_jp2_map(client, tmp_path):
+    """
+    Tests getJP2Image API method with Map with a figure test.
+    """
+    filepath = client.download_jp2('2012/01/01', observatory='SOHO', instrument='MDI', measurement='continuum',
+                                   directory=tmp_path)
+    sunpy.map.Map(filepath).plot()
+
+
 @pytest.mark.remote_data
 def test_download_directory_not_exist_all(client, tmpdir):
     """
     Tests for missing directory.
     """
     fake_dir = os.path.join(str(tmpdir), 'directorynotexist')
     filepath = client.download_jp2('2020/01/01', observatory='SOHO',
```

### Comparing `sunpy-4.1.5/sunpy/net/tests/test_scraper.py` & `sunpy-4.1rc1/sunpy/net/tests/test_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,23 +175,24 @@
     startdate = parse_time((2010, 1, 10, 20, 30))
     enddate = parse_time((2010, 1, 20, 20, 30))
     assert len(s.filelist(TimeRange(startdate, enddate))) == 0
 
 
 @pytest.mark.remote_data
 def testFilesRange_sameDirectory_remote():
-    pattern = ('http://proba2.oma.be/{instrument}/data/bsd/%Y/%m/%d/'
-               '{instrument}_lv1_%Y%m%d_%H%M%S.fits')
+    pattern = ('http://solarmonitor.org/data/%Y/%m/%d/'
+               'fits/{instrument}/'
+               '{instrument}_00174_fd_%Y%m%d_%H%M%S.fts.gz')
     s = Scraper(pattern, instrument='swap')
     startdate = parse_time((2014, 5, 14, 0, 0))
-    enddate = parse_time((2014, 5, 14, 0, 5))
+    enddate = parse_time((2014, 5, 14, 6, 30))
     timerange = TimeRange(startdate, enddate)
     assert len(s.filelist(timerange)) == 2
-    startdate = parse_time((2014, 5, 14, 0, 6))
-    enddate = parse_time((2014, 5, 14, 0, 7))
+    startdate = parse_time((2014, 5, 14, 21, 0))
+    enddate = parse_time((2014, 5, 14, 23, 30))
     timerange = TimeRange(startdate, enddate)
     assert len(s.filelist(timerange)) == 0
 
 
 @pytest.mark.remote_data
 def testFilesRange_sameDirectory_months_remote():
     pattern = ('http://www.srl.caltech.edu/{spacecraft}/DATA/{instrument}/'
@@ -293,15 +294,15 @@
     tr = TimeRange(start, end)
     file_timerange = get_timerange_from_exdict(exdict)
     assert file_timerange == tr
 
 
 @pytest.mark.remote_data
 def test_yearly_overlap():
-    # Check that a time range that falls within the interval that a file represents
+    # Check that a time range that falls within the interval that a file reprsents
     # returns a single result.
     pattern = "https://www.ngdc.noaa.gov/stp/space-weather/solar-data/solar-features/solar-flares/x-rays/goes/xrs/goes-xrs-report_%Y.txt"
     scraper = Scraper(pattern)
 
     # Should return a single file for 2013
     trange = TimeRange("2013-01-02", "2013-01-03")
     assert len(scraper.filelist(trange)) == 1
```

### Comparing `sunpy-4.1.5/sunpy/net/vso/attrs.py` & `sunpy-4.1rc1/sunpy/net/vso/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/vso/data/attrs.json` & `sunpy-4.1rc1/sunpy/net/vso/data/attrs.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9835112747033389%*

 * *Differences: {"'detector'": "{insert: [(13, ['L1', 'Coronado solar telescope L1']), (39, ['L2', 'Coronado solar "*

 * *               "telescope L2'])], delete: [48]}",*

 * * "'instrument'": "{insert: [(35, ['CLIMSO', 'Christian Latouche IMageur SOlaire'])], delete: [61]}",*

 * * "'provider'": "{insert: [(10, ['OMP', 'Observatoire Midi-Pyrénées'])], delete: [4]}",*

 * * "'source'": "{insert: [(34, ['OMP', 'Pic-du-Midi, France'])], delete: [25, 19]}"}*

```diff
@@ -49,14 +49,18 @@
             "7-shell Si detector (flight #1), 7-shell Si detector with collimator (flight #3)"
         ],
         [
             "Hi-C21",
             "High Resolution Coronal Imager 2.1"
         ],
         [
+            "L1",
+            "Coronado solar telescope L1"
+        ],
+        [
             "C1",
             "Coronograph 1"
         ],
         [
             "INNER",
             "None"
         ],
@@ -149,14 +153,18 @@
             "INAF-OACT H\u03b1 and Continuum Detector"
         ],
         [
             "LOI",
             ""
         ],
         [
+            "L2",
+            "Coronado solar telescope L2"
+        ],
+        [
             "VAULT-2014",
             "None"
         ],
         [
             "MEGS-B",
             "Multiple EUV Grating Spectrograph-B"
         ],
@@ -189,18 +197,14 @@
             "Suprathermal Ion Telescope"
         ],
         [
             "FG",
             "None"
         ],
         [
-            "ANDOR_ZYLA-4.2",
-            "Andor Zyla-4.2(VSC-02594) CCD Camera"
-        ],
-        [
             "LFR",
             "None"
         ],
         [
             "SWS",
             "Solar Wind Sector"
         ],
@@ -559,14 +563,18 @@
             "Sun Earth Connection Coronal and Heliospheric Investigation"
         ],
         [
             "EUI",
             "Extreme Ultravoilet Imager"
         ],
         [
+            "CLIMSO",
+            "Christian Latouche IMageur SOlaire"
+        ],
+        [
             "MERGED GONG",
             "None"
         ],
         [
             "LONGWAVE-SLIT-06",
             "Full longwave EUV observation of Sun with EUNIS (trimmed/2006 flight)"
         ],
@@ -663,18 +671,14 @@
             "Soft X-Ray Telescope"
         ],
         [
             "Big Bear",
             "Big Bear Solar Observatory, California TON and GONG+ sites"
         ],
         [
-            "T1-HALPHA",
-            "T1 H\u03b1 Fulldisk"
-        ],
-        [
             "EIT",
             "Extreme ultraviolet Imaging Telescope"
         ],
         [
             "TM-1001",
             "Kanzelh\u00f6he H\u03b1 Pulnix TM-1001 Camera"
         ],
@@ -913,18 +917,14 @@
             "Royal Observatory of Belgium Solar Influences Data Center"
         ],
         [
             "SSC",
             "STEREO Science Center, NASA/Goddard"
         ],
         [
-            "NAOJ",
-            "Solar Science Observatory National Astronomical Observatory of Japan, Mitaka"
-        ],
-        [
             "ESA",
             "European Space Agency"
         ],
         [
             "SDAC",
             "Solar Data Analysis Center, NASA/Goddard"
         ],
@@ -941,14 +941,18 @@
             "High Altitude Observatory, NCAR"
         ],
         [
             "SHA",
             "Stanford Helioseismology Archive, Stanford U."
         ],
         [
+            "OMP",
+            "Observatoire Midi-Pyr\u00e9n\u00e9es"
+        ],
+        [
             "LASP",
             "Laboratory for Atmospheric and Space Physics (University of Colorado at Boulder)"
         ],
         [
             "LSSP",
             "Laboratory for Space and Solar Physics, NASA/Goddard"
         ],
@@ -1067,18 +1071,14 @@
             "Focusing Optics X-ray Solar Imager (flight #1:  11/02/12)"
         ],
         [
             "EUNIS2",
             "None"
         ],
         [
-            "SFT",
-            "Solar Flare Telescope"
-        ],
-        [
             "EUNIS",
             "Extreme Ultraviolet Normal-incidence Spectrograph"
         ],
         [
             "KSO",
             "Kanzelh\u00f6he Solar Observatory, Karl-Franzens-Universit\u00e4t, Graz, Austria"
         ],
@@ -1091,18 +1091,14 @@
             "Reuven Ramaty High Energy Solar Spectroscopic Imager"
         ],
         [
             "ISOON",
             "Improved Solar Observing Optical Network"
         ],
         [
-            "SO2",
-            "None"
-        ],
-        [
             "PSP",
             "Parker Solar Probe"
         ],
         [
             "KPVT",
             "Kitt Peak Vacuum Tower Telescope"
         ],
@@ -1135,14 +1131,18 @@
             "Focusing Optics X-ray Solar Imager (flight #3:  09/07/18)"
         ],
         [
             "CLASP2",
             "Chromospheric LAyer SpectroPolarimeter 2"
         ],
         [
+            "OMP",
+            "Pic-du-Midi, France"
+        ],
+        [
             "MCCD",
             "Mees CCD Imaging Spectrograph"
         ],
         [
             "SDO",
             "Solar Dynamics Observatory"
         ],
```

### Comparing `sunpy-4.1.5/sunpy/net/vso/legacy_response.py` & `sunpy-4.1rc1/sunpy/net/vso/legacy_response.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/net/vso/table_response.py` & `sunpy-4.1rc1/sunpy/net/vso/table_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 has_notime_recs.append(rec)
     has_time_recs = sorted(has_time_recs, key=lambda x: x.time.start)
     all_recs = has_time_recs + has_notime_recs
     return all_recs
 
 
 class VSOQueryResponseTable(QueryResponseTable):
-    hide_keys = ['fileid', 'fileurl', 'Info Required']
+    hide_keys = ['fileid', 'fileurl']
     errors = TableAttribute(default=[])
     size_column = 'Size'
 
     @classmethod
     def from_zeep_response(cls, response, *, client, _sort=True):
         """
         Construct a table response from the zeep response.
@@ -70,36 +70,40 @@
         for record in records:
             row = defaultdict(lambda: None)
             for key, value in serialize_object(record).items():
                 if not isinstance(value, Mapping):
                     if key == "size":
                         # size is in bytes with a very high degree of precision.
                         value = (value * u.Kibyte).to(u.Mibyte).round(5)
+
                     key = key.capitalize() if key not in cls.hide_keys else key
                     row[key] = value
                 else:
                     if key == "wave":
                         # Some records in the VSO have 'kev' which astropy
-                        # doesn't recognize as a unit, so fix it.
+                        # doesn't recognise as a unit, so fix it.
                         waveunit = value['waveunit']
                         waveunit = 'keV' if waveunit == 'kev' else waveunit
+
                         row["Wavelength"] = None
                         if value['wavemin'] is not None and value['wavemax'] is not None:
                             row["Wavelength"] = u.Quantity(
                                 [float(value['wavemin']), float(value['wavemax'])],
                                 unit=waveunit)
+
                         row["Wavetype"] = value['wavetype']
                         continue
                     for subkey, subvalue in value.items():
                         if key == "time" and subvalue is not None:
                             key_template = f"{subkey.capitalize()} {key.capitalize()}"
                         else:
                             key_template = f"{key.capitalize()} {subkey.capitalize()}"
                         row[key_template] = subvalue
             data.append(row)
+
         data = cls(data, client=client)
         # Parse times
         for col in data.colnames:
             if col.endswith('Time'):
                 try:
                     # Try to use a vectorised call to parse_time
                     data[col] = parse_time(data[col])
```

### Comparing `sunpy-4.1.5/sunpy/net/vso/tests/test_attrs.py` & `sunpy-4.1rc1/sunpy/net/vso/tests/test_attrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     w = core_attrs.Wavelength(1.506e16 * u.Hz, 1.506e16 * u.Hz)
     assert int(w.min.to(u.AA, u.equivalencies.spectral()).value) == 199
     w = core_attrs.Wavelength(1.506e7 * u.GHz, 1.506e7 * u.GHz)
     assert int(w.min.to(u.AA, u.equivalencies.spectral()).value) == 199
 
     with pytest.raises(u.UnitsError) as excinfo:
         core_attrs.Wavelength(10 * u.g, 23 * u.g)
-    assert ('This unit is not convertible to any of [Unit("Angstrom"), Unit("kHz"), '
+    assert ('This unit is not convertable to any of [Unit("Angstrom"), Unit("kHz"), '
             'Unit("keV")]' in str(excinfo.value))
 
 
 def test_time_xor():
     one = core_attrs.Time((2010, 1, 1), (2010, 1, 2))
     a = one ^ core_attrs.Time((2010, 1, 1, 1), (2010, 1, 1, 2))
```

### Comparing `sunpy-4.1.5/sunpy/net/vso/tests/test_vso.py` & `sunpy-4.1rc1/sunpy/net/vso/tests/test_vso.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     size_ = table['Size']
     assert len(size_) == 1
     assert size_[0] == 0.0
 
 
 def test_QueryResponse_build_table_with_extent_type(mocker):
     """
-    When explicitly supplying an 'Extent' only the 'type' is stored
+    When explicitly suppling an 'Extent' only the 'type' is stored
     in the built table.
     """
     mocker.patch("sunpy.net.vso.vso.build_client", return_value=True)
     e_type = MockObject(x=1.0, y=2.5, width=37, length=129.2, type='CORONA')
     table = VSOQueryResponseTable.from_zeep_response(MockQRResponse((MockQRRecord(extent=e_type),)),
                                                      client=None)
     extent = table['Extent Type'].data
@@ -355,39 +355,7 @@
 @pytest.mark.remote_data
 def test_iris_filename(client):
     pattern = "/home/yolo/sunpy/data/{file}"
     url = "https://www.lmsal.com/solarsoft/irisa/data/level2_compressed/2018/01/02/20180102_153155_3610108077/iris_l2_20180102_153155_3610108077_SJI_1330_t000.fits.gz"
     search_results = client.search(a.Time("2018-01-02 15:31:55", "2018-01-02 15:31:55"), a.Instrument.iris)
     filename = client.mk_filename(pattern, search_results[0], None, url)
     assert filename.endswith("iris_l2_20180102_153155_3610108077_sji_1330_t000_fits.gz")
-
-
-@pytest.mark.remote_data
-def test_table_noinfo_required(client):
-    res = client.search(a.Time('2017/12/17 00:00:00', '2017/12/17 06:00:00'), a.Instrument('aia'), a.Wavelength(171 * u.angstrom))
-    assert 'Info Required' not in res.keys() and len(res) > 0
-
-
-@pytest.mark.remote_data
-def test_table_has_info_required_swap(client):
-    res = client.search(a.Time('2020/02/15 00:00:00', '2020/02/15 20:00:00'), a.Instrument('swap'), a.Provider('ESA'), a.Source('PROBA2'))
-    assert 'Info Required' in res.keys() and len(res) > 0
-
-
-@pytest.mark.remote_data
-def test_table_has_info_required_lyra(client):
-    res = client.search(a.Time('2020/02/15 00:00:00', '2020/02/17 20:00:00'), a.Instrument('lyra'), a.Provider('ESA'), a.Source('PROBA2'))
-    assert 'Info Required' in res.keys() and len(res) > 0
-
-
-@pytest.mark.remote_data
-def test_fetch_swap(client, tmp_path):
-    res = client.search(a.Time('2020/02/15 00:00:00', '2020/02/15 20:00:00'), a.Instrument('swap'), a.Provider('ESA'), a.Source('PROBA2'))
-    files = client.fetch(res[0:1], path=tmp_path)
-    assert len(files) == 1
-
-
-@pytest.mark.remote_data
-def test_fetch_lyra(client, tmp_path):
-    res = client.search(a.Time('2020/02/15 00:00:00', '2020/02/17 20:00:00'), a.Instrument('lyra'), a.Provider('ESA'), a.Source('PROBA2'))
-    files = client.fetch(res[0:1], path=tmp_path)
-    assert len(files) == 1
```

### Comparing `sunpy-4.1.5/sunpy/net/vso/vso.py` & `sunpy-4.1rc1/sunpy/net/vso/vso.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,23 +414,15 @@
 
         results = downloader.download()
         results += err_results
         results._errors += err_results.errors
         return results
 
     def make_getdatarequest(self, response, methods=None, info=None):
-        """
-        Make datarequest with methods from response.
-        """
-        # Pass back the Apache session ID to the VSO if it exists in the response
-        for item in response:
-            info_required = item.get("Info Required", None)
-            if info_required is not None:
-                info['required'] = item['Info Required']
-
+        """ Make datarequest with methods from response. """
         if methods is None:
             methods = self.method_order + ['URL']
 
         return self.create_getdatarequest(
             {g[0]['Provider']: list(g['fileid']) for g in response.group_by('Provider').groups},
             methods, info
         )
```

### Comparing `sunpy-4.1.5/sunpy/net/vso/zeep_plugins.py` & `sunpy-4.1rc1/sunpy/net/vso/zeep_plugins.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/physics/differential_rotation.py` & `sunpy-4.1rc1/sunpy/physics/differential_rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,35 +283,38 @@
     # The keyword "frame_time" must be explicitly set to "sidereal"
     # when using this function.
     diff_rot_kwargs.update({"frame_time": "sidereal"})
 
     # Calculate the interval between the start and end time
     interval = (new_observer.obstime - coordinate.obstime).to(u.s)
 
-    # Compute Stonyhurst Heliographic coordinates - returns (longitude,
-    # latitude). Points off the limb are returned as nan.
-    heliographic_coordinate = coordinate.transform_to(HeliographicStonyhurst)
-
-    # Compute the differential rotation
-    drot = diff_rot(interval, heliographic_coordinate.lat.to(u.degree), **diff_rot_kwargs)
-
-    # Rotate the input coordinate as seen by the original observer
-    heliographic_rotated = SkyCoord(heliographic_coordinate.lon + drot,
-                                    heliographic_coordinate.lat,
-                                    heliographic_coordinate.radius,
-                                    obstime=coordinate.obstime,
-                                    frame=HeliographicStonyhurst)
-
-    # Calculate where the rotated coordinate appears as seen by new observer
-    # for the coordinate system of the input coordinate.  The translational
-    # motion of the Sun will be ignored for the transformation.
-    frame_newobs = coordinate.frame.replicate_without_data(observer=new_observer,
-                                                           obstime=new_observer.obstime)
-    with transform_with_sun_center():
-        return heliographic_rotated.transform_to(frame_newobs)
+    # Ignore some invalid NaN comparisons within astropy
+    # (fixed in astropy 4.0.1 https://github.com/astropy/astropy/pull/9843)
+    with np.errstate(invalid='ignore'):
+        # Compute Stonyhurst Heliographic co-ordinates - returns (longitude,
+        # latitude). Points off the limb are returned as nan.
+        heliographic_coordinate = coordinate.transform_to(HeliographicStonyhurst)
+
+        # Compute the differential rotation
+        drot = diff_rot(interval, heliographic_coordinate.lat.to(u.degree), **diff_rot_kwargs)
+
+        # Rotate the input co-ordinate as seen by the original observer
+        heliographic_rotated = SkyCoord(heliographic_coordinate.lon + drot,
+                                        heliographic_coordinate.lat,
+                                        heliographic_coordinate.radius,
+                                        obstime=coordinate.obstime,
+                                        frame=HeliographicStonyhurst)
+
+        # Calculate where the rotated co-ordinate appears as seen by new observer
+        # for the co-ordinate system of the input co-ordinate.  The translational
+        # motion of the Sun will be ignored for the transformation.
+        frame_newobs = coordinate.frame.replicate_without_data(observer=new_observer,
+                                                               obstime=new_observer.obstime)
+        with transform_with_sun_center():
+            return heliographic_rotated.transform_to(frame_newobs)
 
 
 def _rotate_submap_edge(smap, pixels, observer, **diff_rot_kwargs):
     """
     Helper function that is used to calculate where the edge of a rectangular
     map move to on rotation.
 
@@ -476,15 +479,15 @@
             # As seen from the map observer, which coordinates are behind the Sun.
             where_off_disk_from_map_observer = rotated_coord.transform_to(
                 Heliocentric(observer=smap.observer_coordinate)).z.value < 0
 
             # Re-project the pixels which are on disk back to location of the original observer
             coordinates_at_map_observer = rotated_coord.transform_to(smap.coordinate_frame)
 
-        # Go back to pixel coordinates
+        # Go back to pixel co-ordinates
         x2, y2 = smap.world_to_pixel(coordinates_at_map_observer)
 
     # Re-stack the data to make it correct output form
     xy2 = np.dstack([x2.T.value.flat, y2.T.value.flat])[0]
     # Set the off disk coordinates to NaN so they are not included in the output image.
     xy2[where_off_disk_from_map_observer.flat] = np.nan
```

### Comparing `sunpy-4.1.5/sunpy/physics/tests/reference/test_differential_rotation.txt` & `sunpy-4.1rc1/sunpy/physics/tests/reference/test_differential_rotation.txt`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/physics/tests/test_differential_rotation.py` & `sunpy-4.1rc1/sunpy/physics/tests/test_differential_rotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,18 @@
     assert dmap.heliographic_longitude == new_observer.lon
 
 
 def test_differential_rotate_observer_straddles_limb(straddles_limb_map):
     # Test a map that straddles the limb - triggers sub full disk branches
     # Rotated map should have a smaller extent in the x - direction
     new_observer = get_earth(straddles_limb_map.date + 48*u.hr)
-    dmap = differential_rotate(straddles_limb_map, observer=new_observer)
+    # Ignore some invalid NaN comparisons within astropy
+    # (fixed in astropy 4.0.1 https://github.com/astropy/astropy/pull/9843)
+    with np.errstate(invalid='ignore'):
+        dmap = differential_rotate(straddles_limb_map, observer=new_observer)
     assert dmap.data.shape[1] < straddles_limb_map.data.shape[1]
     # The output map should have the positional properties of the observer
     assert dmap.date.isot == new_observer.obstime.isot
     assert dmap.heliographic_latitude == new_observer.lat
     assert dmap.heliographic_longitude == new_observer.lon
 
 
@@ -266,16 +269,19 @@
     assert dmap.date.isot == new_time.isot
 
 
 def test_differential_rotate_time_straddles_limb(straddles_limb_map):
     # Test a map that straddles the limb - triggers sub full disk branches
     # Rotated map should have a smaller extent in the x - direction
     new_time = straddles_limb_map.date + 48*u.hr
-    with pytest.warns(UserWarning, match="Using 'time' assumes an Earth-based observer"):
-        dmap = differential_rotate(straddles_limb_map, time=new_time)
+    # Ignore some invalid NaN comparisons within astropy
+    # (fixed in astropy 4.0.1 https://github.com/astropy/astropy/pull/9843)
+    with np.errstate(invalid='ignore'):
+        with pytest.warns(UserWarning, match="Using 'time' assumes an Earth-based observer"):
+            dmap = differential_rotate(straddles_limb_map, time=new_time)
     assert dmap.data.shape[1] < straddles_limb_map.data.shape[1]
     # The output map should have the same time as the new time now.
     assert dmap.date.isot == new_time.isot
 
 
 def test_differential_rotate_time_off_disk(all_off_disk_map):
     # Test a map that is entirely off the disk of the Sun
@@ -360,21 +366,27 @@
         res = _rotate_submap_edge(straddles_limb_map, pixels, observer)
         assert all(res.Tx == (straddles_limb_map.pixel_to_world(pixels[:, 0], pixels[:, 1])).Tx)
         assert all(res.Ty == (straddles_limb_map.pixel_to_world(pixels[:, 0], pixels[:, 1])).Ty)
 
     for this_edge in (1, 2):  # Bottom and left edges do move
         pixels = edges[this_edge]
         res = _rotate_submap_edge(straddles_limb_map, pixels, observer)
-        assert all(res.Tx != (straddles_limb_map.pixel_to_world(pixels[:, 0], pixels[:, 1])).Tx)
-        assert all(res.Ty != (straddles_limb_map.pixel_to_world(pixels[:, 0], pixels[:, 1])).Ty)
+        # Ignore some invalid NaN comparisons within astropy
+        # (fixed in astropy 4.0.1 https://github.com/astropy/astropy/pull/9843)
+        with np.errstate(invalid='ignore'):
+            assert all(res.Tx != (straddles_limb_map.pixel_to_world(pixels[:, 0], pixels[:, 1])).Tx)
+            assert all(res.Ty != (straddles_limb_map.pixel_to_world(pixels[:, 0], pixels[:, 1])).Ty)
 
 
 def test_get_extreme_position():
-    coords = SkyCoord([-1, 0, 1, np.nan]*u.arcsec, [-2, 0, 2, -np.nan]
-                      * u.arcsec, frame=frames.Helioprojective)
+    # Ignore some invalid NaN comparisons within astropy
+    # (fixed in astropy 4.0.1 https://github.com/astropy/astropy/pull/9843)
+    with np.errstate(invalid='ignore'):
+        coords = SkyCoord([-1, 0, 1, np.nan]*u.arcsec, [-2, 0, 2, -np.nan]
+                          * u.arcsec, frame=frames.Helioprojective)
 
     with pytest.warns(RuntimeWarning, match='All-NaN axis encountered'):
         assert _get_extreme_position(coords, 'Tx', operator=np.nanmin) == -1
         assert _get_extreme_position(coords, 'Ty', operator=np.nanmin) == -2
 
         assert _get_extreme_position(coords, 'Tx', operator=np.nanmax) == 1
         assert _get_extreme_position(coords, 'Ty', operator=np.nanmax) == 2
```

### Comparing `sunpy-4.1.5/sunpy/sun/_constants.py` & `sunpy-4.1rc1/sunpy/sun/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides a non-comprehensive collection of solar physical constants.
+This module provies a non-comprehensive collection of solar physical constants.
 """
 # TODO: Need better sources for some constants as well as error values.
 import astropy.constants.astropyconst20 as astrocon
 import astropy.units as u
 from astropy.constants import Constant
 from astropy.time import Time
```

### Comparing `sunpy-4.1.5/sunpy/sun/constants.py` & `sunpy-4.1rc1/sunpy/sun/constants.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/sun/models.py` & `sunpy-4.1rc1/sunpy/sun/models.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/sun/tests/test_constants.py` & `sunpy-4.1rc1/sunpy/sun/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/tests/figure_hashes_mpl_352_ft_261_astropy_51_animators_100.json` & `sunpy-4.1rc1/sunpy/tests/figure_hashes_mpl_352_ft_261_astropy_51_animators_100.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8785714285714286%*

 * *Differences: {"'sunpy.map.tests.test_compositemap.test_peek_composite_map'": "'d459182443472330df9b0dde3bde647479c100f56f45b6321619fbf67810c174'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map'": "'9cdfb6c45bc5a95fa3d08fe1b8fc77a2d4f05ef8218f5bf4c7f50f11c6262f81'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map_colors'": "'20b5cb743ee52a34f7977d538f9dbc8d0266ffed7bcfba00fdc393c660f15ef5'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map_contours'": "'30c14e6f4ef00263494b07c60015 […]*

```diff
@@ -1,21 +1,20 @@
 {
     "sunpy.image.tests.test_transform.test_clipping": "f36c82068789b048d5855315f295e2404c85b0a63ec77de0e294d58b43c9acaf",
     "sunpy.image.tests.test_transform.test_nans": "776e5a2c12bbbff9f5f9de647052cd2ad1be03b39586b91502c8ebba08e87c1b",
-    "sunpy.map.tests.test_compositemap.test_peek_composite_map": "a21143a11c499d95b3618d2f82a6d6e8a3cbad6291ab52b20b218b3f4a03c45b",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map": "41ee9a52dc0fb57edcecf307d3ae5ac110bcedf4542cd666977a482b859c088f",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_colors": "e7c8485e33079fa24914cb4b1c4604e698056153d800554b6a4a9696485f0c30",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_contours": "796d7b9e2e11e8fd4ecb58c0daabba55d9a2090552ceb70e7e8f10b6454be7ce",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linestyles": "70b8adf96f2893c110069991f7bfc992863934a0bf9629fcd51a0809a9801382",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linewidths": "fb1edca012f7bd18035863eb077f2c7963d0a13010c5d6c054f91b8e0a9b5c66",
-    "sunpy.map.tests.test_compositemap.test_set_alpha_composite_map": "2b2a157405dc296d5c06c74f7d8bc6e03b3cff4512cf9b0e66a773827497f37a",
-    "sunpy.map.tests.test_map_factory.test_map_jp2_HMI": "3b731f25ab5777f187def8296fbed88d27809867405e0e97d5e808ca1bb4b42c",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[opencv]": "cd86fb9c0ed0e26eaae00d816d0b5d3f381b2be22b8e99d45afe5a511ccd55e5",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scikit-image]": "17748c119a97c112e77fcb368af595f2b5faada067a7188abe846c7b160f9ea8",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scipy]": "9168fca9a4e04def3da12624196b29ebe954004ad269faa4bab11276a85366af",
+    "sunpy.map.tests.test_compositemap.test_peek_composite_map": "d459182443472330df9b0dde3bde647479c100f56f45b6321619fbf67810c174",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map": "9cdfb6c45bc5a95fa3d08fe1b8fc77a2d4f05ef8218f5bf4c7f50f11c6262f81",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_colors": "20b5cb743ee52a34f7977d538f9dbc8d0266ffed7bcfba00fdc393c660f15ef5",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_contours": "30c14e6f4ef00263494b07c600155e7698bbecdfc1925bd4cda9bc824ead1eec",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linestyles": "9cef7e320ddb45e6fc8022acfe2d9c304e07e094474b0bd9e486de1ad2d77f4a",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linewidths": "89d0f1b75b833e48f7cd6a6776929af440764c2e615947270701afaca0e766d4",
+    "sunpy.map.tests.test_compositemap.test_set_alpha_composite_map": "f811cf6be8abfcd1b3a7f4bae7781806b37b1b2b0cb77ac34c4ed4491a1d633a",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[opencv]": "369c75feab7a0b1ebe65bd0ec9084b3c941db45445d88c667311d81f01101afe",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scikit-image]": "27862d38a9ab0c5e61229737e5fe0af962d94ee421e7d5acd2e14c7018bdde44",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scipy]": "4184d5536f49d2811803ba831e212a7708046f4cb2c9fca1252a017fa9d90127",
     "sunpy.map.tests.test_mapbase.test_rotation_rect_pixelated_data": "5b37819c36a50a2a7a26944a2f1481027dd17390e73158f6b5510034102d35bb",
     "sunpy.map.tests.test_mapsequence.test_map_sequence_plot": "3cdc53f41914028a4e9f23112d7e616ce8a423ef5670c8365fdadbc0e59780ca",
     "sunpy.map.tests.test_mapsequence.test_map_sequence_plot_custom_cmap_norm": "c1276702147f4debaa14c17f6b0b2ab7f9e0b1ace309c72e767b2af071c4405e",
     "sunpy.map.tests.test_mapsequence.test_norm_animator": "5a7217dd55ab3a593a27741fecfe0851208fd1d31baeca4cbd018d65aaf3f483",
     "sunpy.map.tests.test_plotting.test_draw_contours_aia": "2ff44dd84d067bf65d541422c62d2152057d170a41dbb44b1ffb8d8d4113c6c8",
     "sunpy.map.tests.test_plotting.test_draw_contours_different_wcs": "90552cdeaf0c4b14e3e758628502b0b0fc7b6c4490763c4bd4849de0ee7df917",
     "sunpy.map.tests.test_plotting.test_draw_grid_aia171": "51c9e572c5708a2112445426bfcaef25650e294b23f3ebd3aa3769d596e57dda",
@@ -29,16 +28,15 @@
     "sunpy.map.tests.test_plotting.test_peek_grid_aia171": "d27ca38c6f529a415a14624dd43ff6a9436b6972d1d82faa4a9884fd601eb106",
     "sunpy.map.tests.test_plotting.test_peek_grid_limb_aia171": "6abc117f65bd55acceaed9ddeddaef34e4f1bf920f86cc4f701f9c87d7bb1845",
     "sunpy.map.tests.test_plotting.test_peek_grid_spacing_aia171": "e2629577592c46e2baa1658fcf1f92ac1e5e6985a08c7aa6d2df3869f4654924",
     "sunpy.map.tests.test_plotting.test_peek_limb_aia171": "2d5a36e6b8873ded8a6141b60caddd9aa697344c8df59852e80c4dcda7fd67be",
     "sunpy.map.tests.test_plotting.test_plot_aia171": "3cdc53f41914028a4e9f23112d7e616ce8a423ef5670c8365fdadbc0e59780ca",
     "sunpy.map.tests.test_plotting.test_plot_aia171_clip": "920852d09b1b0af6ed406312e8e54ce2b327d38061a0652d95df03b41e1c552d",
     "sunpy.map.tests.test_plotting.test_plot_aia171_superpixel": "1c133f41c740f4974b8dd27477a247a64c7f8e387d1d8d8c9b4f42ca0387b2ac",
-    "sunpy.map.tests.test_plotting.test_plot_autoalign": "352a8c7ece7f3439750a199cfa345d1ef23e6c14d545a94f67a6eb2e2257e898",
-    "sunpy.map.tests.test_plotting.test_plot_autoalign_pixel_alignment": "03e6e20d752c9de9f45022ea1819ca9bbd95950b0852f9138b28448636d533b6",
+    "sunpy.map.tests.test_plotting.test_plot_autoalign": "c67e3bd35e56fff7f2e65e7c0fa7b560f468cd60ceac2fa054a3446746e6442e",
     "sunpy.map.tests.test_plotting.test_plot_masked_aia171": "8acfaf714eca9295e1d4ecd17e6eec62c8fc991cba45eeb0ba6d2efaa492d29b",
     "sunpy.map.tests.test_plotting.test_plot_masked_aia171_superpixel": "ffabe0ca544b93c8084af36edb5b293cdce613d13b73ddeaa906ddf2617da34b",
     "sunpy.map.tests.test_plotting.test_plot_resample": "351baa39339b9f7d206232b9c2fb777d7edf965e1554040171ac40e3a1f5ec62",
     "sunpy.map.tests.test_plotting.test_plot_rotated_aia171": "9df0409afa257ebe481aa5170321072ddca349fe596f3d662208e127f39a938e",
     "sunpy.map.tests.test_plotting.test_plot_superpixel": "4fcd7af5690bbb5a1ae65ab2bf80db31aa41f240456cddaf49c6132fd459b973",
     "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right": "e55f63d480032009779aa5c1742aff30694587f8bee2f8201c7c64192880cecb",
     "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right_different_axes": "893064c44b850aea39b24b2a94af10af340745c0e32b867033b0f14684bf337f",
@@ -47,14 +45,15 @@
     "sunpy.map.tests.test_plotting.test_quadrangle_aia17_width_height": "89f18bf54f0ebeb6ce36522620f6551457bfd1dd1da1634edb50cbea5adc2939",
     "sunpy.map.tests.test_plotting.test_rectangle_aia171_top_right": "643d623d94d9390a94266e1088dacb03bd62668815a3b04e1bda51afa701d8a4",
     "sunpy.map.tests.test_plotting.test_rectangle_aia171_width_height": "d6afbac82891ed231d8bcbe5a66fe0098856dba4aca684073ddee2ec3b10a289",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hgs": "c1dc26bedf3d24690364637e1a7d6fde165445049e633e8407ad2ccf42416fcb",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_adaptive": "40cb43b7431941e8977449f5ed5d1439e7dddf9f0ec0aa21d0c18f09a25e259c",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_exact": "93171456dfac771f53bc0465922cf5811048df0b56100d329a55f71b36bdc8f5",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_interpolation": "b82e6462d4ccb8c188b5f6deac3258326ba6840ef624c18f044a9d4cadce3cf2",
+    "sunpy.net.tests.test_helioviewer.test_download_jp2_map": "a71654a4a7ceea689869c68f4cd7f0ebfc5e970caed73f2e73e677745c99e0e0",
     "sunpy.timeseries.sources.tests.test_eve.test_esp_peek": "28b1e7af0e1894d22fd9db90d9e2bc5eb76e291c9e41fa1bb1d33d95bd13cce3",
     "sunpy.timeseries.sources.tests.test_eve.test_eve_peek": "2a22f93af44971411800e4fcd0d93d2128fe2b9e6b97e576e8372c2cd12d7d78",
     "sunpy.timeseries.sources.tests.test_fermi_gbm.test_fermi_gbm_peek": "83f0b53ca6f1cd809bd03e4aff80b3c02c8078e552b0c3e90b2cb3cf26932a51",
     "sunpy.timeseries.sources.tests.test_goes.test_goes_peek": "4fc2d89d3ce2727a75a9feee13c0671e4bd570fe87af2d1706d13a2799db3ee3",
     "sunpy.timeseries.sources.tests.test_goes.test_goes_ylim": "432cd4458eed29764d6bfaae2bee0820706fc293d7b23972fc587eae590bcd72",
     "sunpy.timeseries.sources.tests.test_lyra.test_lyra_peek": "48924d42773a4d834342cdce5ad1e005db9980bf6db6525d97a141a08f411aba",
     "sunpy.timeseries.sources.tests.test_noaa.test_noaa_json_ind_peek": "a61ea2eb004d89f16b6ea4b6c56b2eedbb456ecc301d2c710eb3312f70c6a6f7",
```

### Comparing `sunpy-4.1.5/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json` & `sunpy-4.1rc1/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8714285714285714%*

 * *Differences: {"'sunpy.map.tests.test_compositemap.test_peek_composite_map'": "'d459182443472330df9b0dde3bde647479c100f56f45b6321619fbf67810c174'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map'": "'9cdfb6c45bc5a95fa3d08fe1b8fc77a2d4f05ef8218f5bf4c7f50f11c6262f81'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map_colors'": "'20b5cb743ee52a34f7977d538f9dbc8d0266ffed7bcfba00fdc393c660f15ef5'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map_contours'": "'30c14e6f4ef00263494b07c60015 […]*

```diff
@@ -1,21 +1,20 @@
 {
     "sunpy.image.tests.test_transform.test_clipping": "f36c82068789b048d5855315f295e2404c85b0a63ec77de0e294d58b43c9acaf",
     "sunpy.image.tests.test_transform.test_nans": "776e5a2c12bbbff9f5f9de647052cd2ad1be03b39586b91502c8ebba08e87c1b",
-    "sunpy.map.tests.test_compositemap.test_peek_composite_map": "a21143a11c499d95b3618d2f82a6d6e8a3cbad6291ab52b20b218b3f4a03c45b",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map": "41ee9a52dc0fb57edcecf307d3ae5ac110bcedf4542cd666977a482b859c088f",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_colors": "e7c8485e33079fa24914cb4b1c4604e698056153d800554b6a4a9696485f0c30",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_contours": "796d7b9e2e11e8fd4ecb58c0daabba55d9a2090552ceb70e7e8f10b6454be7ce",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linestyles": "70b8adf96f2893c110069991f7bfc992863934a0bf9629fcd51a0809a9801382",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linewidths": "fb1edca012f7bd18035863eb077f2c7963d0a13010c5d6c054f91b8e0a9b5c66",
-    "sunpy.map.tests.test_compositemap.test_set_alpha_composite_map": "2b2a157405dc296d5c06c74f7d8bc6e03b3cff4512cf9b0e66a773827497f37a",
-    "sunpy.map.tests.test_map_factory.test_map_jp2_HMI": "3b731f25ab5777f187def8296fbed88d27809867405e0e97d5e808ca1bb4b42c",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[opencv]": "cd86fb9c0ed0e26eaae00d816d0b5d3f381b2be22b8e99d45afe5a511ccd55e5",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scikit-image]": "17748c119a97c112e77fcb368af595f2b5faada067a7188abe846c7b160f9ea8",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scipy]": "9168fca9a4e04def3da12624196b29ebe954004ad269faa4bab11276a85366af",
+    "sunpy.map.tests.test_compositemap.test_peek_composite_map": "d459182443472330df9b0dde3bde647479c100f56f45b6321619fbf67810c174",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map": "9cdfb6c45bc5a95fa3d08fe1b8fc77a2d4f05ef8218f5bf4c7f50f11c6262f81",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_colors": "20b5cb743ee52a34f7977d538f9dbc8d0266ffed7bcfba00fdc393c660f15ef5",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_contours": "30c14e6f4ef00263494b07c600155e7698bbecdfc1925bd4cda9bc824ead1eec",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linestyles": "9cef7e320ddb45e6fc8022acfe2d9c304e07e094474b0bd9e486de1ad2d77f4a",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linewidths": "89d0f1b75b833e48f7cd6a6776929af440764c2e615947270701afaca0e766d4",
+    "sunpy.map.tests.test_compositemap.test_set_alpha_composite_map": "f811cf6be8abfcd1b3a7f4bae7781806b37b1b2b0cb77ac34c4ed4491a1d633a",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[opencv]": "369c75feab7a0b1ebe65bd0ec9084b3c941db45445d88c667311d81f01101afe",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scikit-image]": "27862d38a9ab0c5e61229737e5fe0af962d94ee421e7d5acd2e14c7018bdde44",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scipy]": "4184d5536f49d2811803ba831e212a7708046f4cb2c9fca1252a017fa9d90127",
     "sunpy.map.tests.test_mapbase.test_rotation_rect_pixelated_data": "5b37819c36a50a2a7a26944a2f1481027dd17390e73158f6b5510034102d35bb",
     "sunpy.map.tests.test_mapsequence.test_map_sequence_plot": "3cdc53f41914028a4e9f23112d7e616ce8a423ef5670c8365fdadbc0e59780ca",
     "sunpy.map.tests.test_mapsequence.test_map_sequence_plot_custom_cmap_norm": "c1276702147f4debaa14c17f6b0b2ab7f9e0b1ace309c72e767b2af071c4405e",
     "sunpy.map.tests.test_mapsequence.test_norm_animator": "5a7217dd55ab3a593a27741fecfe0851208fd1d31baeca4cbd018d65aaf3f483",
     "sunpy.map.tests.test_plotting.test_draw_contours_aia": "2ff44dd84d067bf65d541422c62d2152057d170a41dbb44b1ffb8d8d4113c6c8",
     "sunpy.map.tests.test_plotting.test_draw_contours_different_wcs": "90552cdeaf0c4b14e3e758628502b0b0fc7b6c4490763c4bd4849de0ee7df917",
     "sunpy.map.tests.test_plotting.test_draw_grid_aia171": "51c9e572c5708a2112445426bfcaef25650e294b23f3ebd3aa3769d596e57dda",
@@ -29,16 +28,15 @@
     "sunpy.map.tests.test_plotting.test_peek_grid_aia171": "d27ca38c6f529a415a14624dd43ff6a9436b6972d1d82faa4a9884fd601eb106",
     "sunpy.map.tests.test_plotting.test_peek_grid_limb_aia171": "6abc117f65bd55acceaed9ddeddaef34e4f1bf920f86cc4f701f9c87d7bb1845",
     "sunpy.map.tests.test_plotting.test_peek_grid_spacing_aia171": "e2629577592c46e2baa1658fcf1f92ac1e5e6985a08c7aa6d2df3869f4654924",
     "sunpy.map.tests.test_plotting.test_peek_limb_aia171": "2d5a36e6b8873ded8a6141b60caddd9aa697344c8df59852e80c4dcda7fd67be",
     "sunpy.map.tests.test_plotting.test_plot_aia171": "3cdc53f41914028a4e9f23112d7e616ce8a423ef5670c8365fdadbc0e59780ca",
     "sunpy.map.tests.test_plotting.test_plot_aia171_clip": "920852d09b1b0af6ed406312e8e54ce2b327d38061a0652d95df03b41e1c552d",
     "sunpy.map.tests.test_plotting.test_plot_aia171_superpixel": "1c133f41c740f4974b8dd27477a247a64c7f8e387d1d8d8c9b4f42ca0387b2ac",
-    "sunpy.map.tests.test_plotting.test_plot_autoalign": "352a8c7ece7f3439750a199cfa345d1ef23e6c14d545a94f67a6eb2e2257e898",
-    "sunpy.map.tests.test_plotting.test_plot_autoalign_pixel_alignment": "03e6e20d752c9de9f45022ea1819ca9bbd95950b0852f9138b28448636d533b6",
+    "sunpy.map.tests.test_plotting.test_plot_autoalign": "c67e3bd35e56fff7f2e65e7c0fa7b560f468cd60ceac2fa054a3446746e6442e",
     "sunpy.map.tests.test_plotting.test_plot_masked_aia171": "8acfaf714eca9295e1d4ecd17e6eec62c8fc991cba45eeb0ba6d2efaa492d29b",
     "sunpy.map.tests.test_plotting.test_plot_masked_aia171_superpixel": "ffabe0ca544b93c8084af36edb5b293cdce613d13b73ddeaa906ddf2617da34b",
     "sunpy.map.tests.test_plotting.test_plot_resample": "351baa39339b9f7d206232b9c2fb777d7edf965e1554040171ac40e3a1f5ec62",
     "sunpy.map.tests.test_plotting.test_plot_rotated_aia171": "9df0409afa257ebe481aa5170321072ddca349fe596f3d662208e127f39a938e",
     "sunpy.map.tests.test_plotting.test_plot_superpixel": "4fcd7af5690bbb5a1ae65ab2bf80db31aa41f240456cddaf49c6132fd459b973",
     "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right": "e55f63d480032009779aa5c1742aff30694587f8bee2f8201c7c64192880cecb",
     "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right_different_axes": "893064c44b850aea39b24b2a94af10af340745c0e32b867033b0f14684bf337f",
@@ -47,25 +45,26 @@
     "sunpy.map.tests.test_plotting.test_quadrangle_aia17_width_height": "89f18bf54f0ebeb6ce36522620f6551457bfd1dd1da1634edb50cbea5adc2939",
     "sunpy.map.tests.test_plotting.test_rectangle_aia171_top_right": "643d623d94d9390a94266e1088dacb03bd62668815a3b04e1bda51afa701d8a4",
     "sunpy.map.tests.test_plotting.test_rectangle_aia171_width_height": "d6afbac82891ed231d8bcbe5a66fe0098856dba4aca684073ddee2ec3b10a289",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hgs": "c1dc26bedf3d24690364637e1a7d6fde165445049e633e8407ad2ccf42416fcb",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_adaptive": "40cb43b7431941e8977449f5ed5d1439e7dddf9f0ec0aa21d0c18f09a25e259c",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_exact": "93171456dfac771f53bc0465922cf5811048df0b56100d329a55f71b36bdc8f5",
     "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_interpolation": "b82e6462d4ccb8c188b5f6deac3258326ba6840ef624c18f044a9d4cadce3cf2",
+    "sunpy.net.tests.test_helioviewer.test_download_jp2_map": "a71654a4a7ceea689869c68f4cd7f0ebfc5e970caed73f2e73e677745c99e0e0",
     "sunpy.timeseries.sources.tests.test_eve.test_esp_peek": "28b1e7af0e1894d22fd9db90d9e2bc5eb76e291c9e41fa1bb1d33d95bd13cce3",
     "sunpy.timeseries.sources.tests.test_eve.test_eve_peek": "2a22f93af44971411800e4fcd0d93d2128fe2b9e6b97e576e8372c2cd12d7d78",
     "sunpy.timeseries.sources.tests.test_fermi_gbm.test_fermi_gbm_peek": "83f0b53ca6f1cd809bd03e4aff80b3c02c8078e552b0c3e90b2cb3cf26932a51",
     "sunpy.timeseries.sources.tests.test_goes.test_goes_peek": "4fc2d89d3ce2727a75a9feee13c0671e4bd570fe87af2d1706d13a2799db3ee3",
     "sunpy.timeseries.sources.tests.test_goes.test_goes_ylim": "432cd4458eed29764d6bfaae2bee0820706fc293d7b23972fc587eae590bcd72",
     "sunpy.timeseries.sources.tests.test_lyra.test_lyra_peek": "48924d42773a4d834342cdce5ad1e005db9980bf6db6525d97a141a08f411aba",
     "sunpy.timeseries.sources.tests.test_noaa.test_noaa_json_ind_peek": "a61ea2eb004d89f16b6ea4b6c56b2eedbb456ecc301d2c710eb3312f70c6a6f7",
     "sunpy.timeseries.sources.tests.test_noaa.test_noaa_json_pre_peek": "2673bf752a5f4133239a4b96308de5159e1202ce55efa5a590deba213788af74",
     "sunpy.timeseries.sources.tests.test_norh.test_norh_peek": "a403f6ec3064a1dbcf4c190a9724d3b893b4608ca5d0a0cae8a400378f0c8f9e",
     "sunpy.timeseries.sources.tests.test_rhessi.test_rhessi_peek": "f7783ff9d1b00a03cebfdc173057f67a44de00621eff3bb22d23355c3ba7c85b",
     "sunpy.timeseries.tests.test_timeseriesbase.test_column_subset_peek": "0c1ac6714d9bc505db3ee449fa9a8ba6842b0d756a8c8f02a2133547123c2a92",
     "sunpy.timeseries.tests.test_timeseriesbase.test_generic_ts_peek": "ba0469ba921c3367384c04de4e64d16cacd1499277a14f1809c087d8f21ee041",
     "sunpy.visualization.animator.tests.test_mapsequenceanimator.test_map_sequence_animator_wcs_simple_plot": "5f52fb6efb00e04e4de394ec8d5edb940d5690602ff249998631eacef3b9f2f1",
-    "sunpy.visualization.colormaps.tests.test_cm.test_cmap_visual": "fbbd93e66471a92f042543226f7e091f3c3b7f6079bbf418863019e63aaa4db9",
+    "sunpy.visualization.colormaps.tests.test_cm.test_cmap_visual": "3e05e268e324b58493ec692a48c757a7f6ed5e1a4744b03066ff7a72bdda96e7",
     "sunpy.visualization.tests.test_drawing.test_draw_equator_aia171": "abc52d5e8254b32ed42942926a4ee92d7b0aaf441bfe8c54cdcd98d6a7a62eba",
     "sunpy.visualization.tests.test_drawing.test_draw_prime_meridian_aia171": "6602b10b71759a5dae32691cfdab8762de61409a433c97b151de663f3515eb66",
     "sunpy.visualization.tests.test_drawing.test_heliographic_equator_prime_meridian": "3cb195a44e899ef46de7365bd0a0c580b7ea69662bdc560a1bbb1686c2ad48cf"
 }
```

### Comparing `sunpy-4.1.5/sunpy/tests/helpers.py` & `sunpy-4.1rc1/sunpy/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/tests/mocks.py` & `sunpy-4.1rc1/sunpy/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/tests/self_test.py` & `sunpy-4.1rc1/sunpy/tests/self_test.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/tests/tests/test_mocks.py` & `sunpy-4.1rc1/sunpy/tests/tests/test_mocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """
     rd_wr = MockOpenTextFile(mode='r+')
 
     assert rd_wr.name == 'N/A'
     assert rd_wr.readable() is True
     assert rd_wr.writable() is True
 
-    # Initially empty
+    # Initailly empty
     assert rd_wr.read() == ''
 
     data = '0123456789'
 
     num_chars = rd_wr.write(data)
     assert num_chars == len(data)
```

### Comparing `sunpy-4.1.5/sunpy/tests/tests/test_self_test.py` & `sunpy-4.1rc1/sunpy/tests/tests/test_self_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 
 def test_main_figure_only(monkeypatch):
     args = _self_test_args(figure_only=True)
     assert args == ['-W', 'ignore', '--pyargs', 'sunpy', '-m', 'mpl_image_compare']
 
 
 def test_warnings():
-    # Ensure that our warning trickery doesn't stop pytest.warns working
+    # Ensure that our warning trickery dosen't stop pytest.warns working
     with pytest.warns(SunpyDeprecationWarning):
         warn_deprecated("Hello")
```

### Comparing `sunpy-4.1.5/sunpy/tests/tests/test_sunpy_data_filenames.py` & `sunpy-4.1rc1/sunpy/tests/tests/test_sunpy_data_filenames.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/time/tests/test_taiseconds.py` & `sunpy-4.1rc1/sunpy/time/tests/test_taiseconds.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/time/tests/test_time.py` & `sunpy-4.1rc1/sunpy/time/tests/test_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,21 @@
 def test_parse_time_24_2():
     dt = parse_time("2010-10-10T24:00:00.000000")
     assert dt == Time('2010-10-11')
     assert dt.format == 'isot'
     assert dt.scale == 'utc'
 
 
-def test_parse_time_microseconds_excess_trailing_zeros():
-    dt = parse_time('2010-Oct-10 00:00:00.1234560')
-    assert dt == Time('2010-10-10 00:00:00.123456')
+def test_parse_time_trailing_zeros():
+    # see issue #289 at https://github.com/sunpy/sunpy/issues/289
+    dt = parse_time('2010-10-10T00:00:00.00000000')
+    assert dt == Time('2010-10-10')
     assert dt.format == 'isot'
     assert dt.scale == 'utc'
 
-    # Excess digits beyond 6 digits should error if they are not zeros
-    with pytest.raises(ValueError):
-        dt = parse_time('2010-Oct-10 00:00:00.1234567')
-
-    # An ending run of zeros should still error if they are not a microsecond field
-    with pytest.raises(ValueError):
-        dt = parse_time('10-Oct-2010.0000000')
-
 
 def test_parse_time_tuple():
     dt = parse_time((1966, 2, 3))
     assert dt == LANDING
     assert dt.format == 'isot'
     assert dt.scale == 'utc'
```

### Comparing `sunpy-4.1.5/sunpy/time/tests/test_timerange.py` & `sunpy-4.1rc1/sunpy/time/tests/test_timerange.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/time/time.py` & `sunpy-4.1rc1/sunpy/time/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides a collection of time handing functions.
+This module provies a collection of time handing functions.
 """
 import re
 import textwrap
 from datetime import date, datetime
 from functools import singledispatch
 
 import numpy as np
@@ -45,22 +45,20 @@
     "%Y%m%dT%H%M%S",  # Example 20070504T210812
     "%Y/%m/%d %H:%M:%S",  # Example 2007/05/04 21:08:12
     "%Y/%m/%d %H:%M",  # Example 2007/05/04 21:08
     "%Y/%m/%d %H:%M:%S.%f",  # Example 2007/05/04 21:08:12.999999
     "%Y-%m-%d %H:%M:%S.%f",  # Example 2007-05-04 21:08:12.999999
     "%Y-%m-%d %H:%M:%S",  # Example 2007-05-04 21:08:12
     "%Y-%m-%d %H:%M",  # Example 2007-05-04 21:08
-    "%Y-%b-%d %H:%M:%S.%f",  # Example 2007-May-04 21:08:12.999999
     "%Y-%b-%d %H:%M:%S",  # Example 2007-May-04 21:08:12
     "%Y-%b-%d %H:%M",  # Example 2007-May-04 21:08
     "%Y-%b-%d",  # Example 2007-May-04
     "%Y-%m-%d",  # Example 2007-05-04
     "%Y/%m/%d",  # Example 2007/05/04
     "%d-%b-%Y",  # Example 04-May-2007
-    "%d-%b-%Y %H:%M:%S",  # Example 04-May-2007 21:08:12
     "%d-%b-%Y %H:%M:%S.%f",  # Example 04-May-2007 21:08:12.999999
     "%Y%m%d_%H%M%S",  # Example 20070504_210812
     "%Y:%j:%H:%M:%S",  # Example 2012:124:21:08:12
     "%Y:%j:%H:%M:%S.%f",  # Example 2012:124:21:08:12.999999
     "%Y%m%d%H%M%S",  # Example 20140101000001 (JSOC/VSO Export/Downloads)
     "%Y.%m.%d_%H:%M:%S_TAI",  # Example 2016.05.04_21:08:12_TAI - JSOC
     "%Y.%m.%d_%H:%M:%S_UTC",  # Example 2016.05.04_21:08:12_UTC - JSOC
@@ -100,36 +98,26 @@
     # from 24:00:00 to 00:00:00 the next day because strptime does not
     # understand the former.
     for key, value in REGEX.items():
         format = format.replace(key, value)
     match = re.match(format, inp)
     if match is None:
         return None, None
-
-    found_groups = match.groupdict()
-
-    # Special handling to strip any excess zeros beyond the six digits of the microsecond field
-    if "microsecond" in found_groups and re.match(r"\d{6}0+", match.group("microsecond")):
-        from_, to = match.span("microsecond")
-        inp = inp[:from_] + match.group("microsecond")[:6] + inp[to:]
-        match = re.match(format, inp)
-
-    # Special handling to add a day if the hour is 24 and the minute/second/microsecond are all zero
-    add_one_day = False
-    if "hour" in found_groups and match.group("hour") == "24":
+    try:
+        hour = match.group("hour")
+    except IndexError:
+        return inp, False
+    if hour == "24":
         if not all(
                 _n_or_eq(_group_or_none(match, g, int), 00)
                 for g in ["minute", "second", "microsecond"]):
             raise ValueError
         from_, to = match.span("hour")
-        inp = inp[:from_] + "00" + inp[to:]
-        add_one_day = True
-        match = re.match(format, inp)
-
-    return inp, add_one_day
+        return inp[:from_] + "00" + inp[to:], True
+    return inp, False
 
 
 def find_time(string, format):
     """
     Return iterator of occurrences of date formatted with format in string.
 
     Currently supported format codes:
@@ -223,14 +211,19 @@
 
     # Otherwise return the default method
     return convert_time.dispatch(object)(time_list, format, **kwargs)
 
 
 @convert_time.register(str)
 def convert_time_str(time_string, **kwargs):
+    # remove trailing zeros and the final dot to allow any
+    # number of zeros. This solves issue #289
+    if '.' in time_string:
+        time_string = time_string.rstrip("0").rstrip(".")
+
     if 'TAI' in time_string:
         kwargs['scale'] = 'tai'
 
     for time_format in TIME_FORMAT_LIST:
         try:
             try:
                 ts, add_one_day = _regex_parse_time(time_string, time_format)
@@ -241,15 +234,15 @@
             t = Time.strptime(ts, time_format, **kwargs)
             if add_one_day:
                 t += _ONE_DAY_TIMEDELTA
             return t
         except ValueError:
             pass
 
-    # when no format matches, call default function
+    # when no format matches, call default fucntion
     return convert_time.dispatch(object)(time_string, **kwargs)
 
 
 def _get_time_fmt(time_string):
     """
     Try all the formats in TIME_FORMAT_LIST to work out which one applies to
     the time string.
```

### Comparing `sunpy-4.1.5/sunpy/time/timeformats.py` & `sunpy-4.1rc1/sunpy/time/timeformats.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,17 @@
 
 class TimeUTime(TimeFromEpoch):
     """
     UT seconds from 1979-01-01 00:00:00 UTC, ignoring leap seconds.
 
     Notes
     -----
-    This format "ignores" leap seconds by treating each day as spanned by exactly
-    86400 seconds, which means that this format's second is not actually uniform in
-    duration.  On a day without a leap second, this format's second is equal to an
-    SI second.  On a day with a leap second, this format's second is larger than an
-    SI second by 1/86400 of an SI second.
-
-    This format is very similar to the default output format of the ``anytim``
-    routine in SSW in that there are exactly 86400 seconds assigned for each day.
-    However, ``anytim`` treats the seconds as always equal to an SI second, and thus
-    the 86400 seconds span only the first 86400/86401 of the day, and the leap
-    second is skipped over.  This results in discrepancies of up to a second on days
-    with a leap second.
+    This format is very similar to the default output format of the the ``anytim``
+    routine in SSW.  However, there are discrepancies of up to a second on days with
+    a leap second.
 
     This format is equivalent to `~astropy.time.TimeUnix`, except that the epoch is
     9 years later.
 
     References
     ----------
     * `anytim routine in SSW <https://hesperia.gsfc.nasa.gov/ssw/gen/idl/utplot/anytim.pro>`_
```

### Comparing `sunpy-4.1.5/sunpy/time/timerange.py` & `sunpy-4.1rc1/sunpy/time/timerange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides an object that can handle a time range.
+This module provies a object that can handle a time range.
 """
 from datetime import timedelta
 
 import astropy.units as u
 from astropy.time import Time, TimeDelta
 
 from sunpy import config
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/metadata.py` & `sunpy-4.1rc1/sunpy/timeseries/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides metadata support for `~sunpy.timeseries.TimeSeries`.
+This module provies metadata support for `~sunpy.timeseries.TimeSeries`.
 """
 import copy
 import itertools
 from collections.abc import Iterable
 
 from sunpy.time import TimeRange, parse_time
 from sunpy.time.time import _variables_for_parse_time_docstring
@@ -394,15 +394,15 @@
             Defaults to `False`
         """
         # Find all matching metadata entries
         indices = self.find_indices(time=time, colname=colname)
 
         # Now update each matching entries
         for i in indices:
-            # Separate keys for new and current pairs
+            # Seperate keys for new and current pairs
             old_keys = set(dictionary.keys())
             old_keys.intersection_update(set(self.metadata[i][2].keys()))
             new_keys = set(dictionary.keys())
             new_keys.difference_update(old_keys)
 
             # Old keys only overwritten if allowed
             for key in (self.metadata[i][2].keys()):
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/__init__.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides a collection of datasource-specific
+This module provies a collection of datasource-specific
 `~sunpy.timeseries.TimeSeries` classes.
 
 Each mission should have its own file with one or more classes defined.
 Typically, these classes will be subclasses of the
 `sunpy.timeseries.TimeSeries`.
 """
 from sunpy.timeseries.sources.eve import ESPTimeSeries, EVESpWxTimeSeries
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/eve.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/eve.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     which is part of the Extreme ultraviolet Variability Experiment (EVE) on board
     SDO. ESP provides high time cadence (0.25s) EUV irradiance measurements in five
     channels, one soft X-ray and 4 EUV. The first four orders of the diffraction grating
     gives measurements centered on 18nm, 26nm, 30nm and 36nm. The zeroth order (obtained
     by 4 photodiodes) provides the soft X-ray measurements from 0.1-7nm.
 
     The ESP level 1 fits files are fully calibrated. The TimeSeries object created from
-    an ESP fits file will contain 4 columns namely:
+    an ESP fits file will conatain 4 columns namely:
 
         * 'QD' - sum of 4 quad diodes, this is the soft X-ray measurements 0.1-7nm
         * 'CH_18' - EUV irradiance 18nm
         * 'CH_26' - EUV irradiance 26nm
         * 'CH_30' - EUV irradiance 30nm
         * 'CH_36' - EUV irradiance 36nm
 
@@ -185,15 +185,15 @@
     >>> eve.peek(subplots=True)  # doctest: +SKIP
 
     References
     ----------
     * `SDO Mission Homepage <https://sdo.gsfc.nasa.gov/>`__
     * `EVE Homepage <http://lasp.colorado.edu/home/eve/>`__
     * `Level 0CS Definition <http://lasp.colorado.edu/home/eve/data/>`__
-    * `EVE Data Access <http://lasp.colorado.edu/home/eve/data/data-access/>`__
+    * `EVE Data Acess <http://lasp.colorado.edu/home/eve/data/data-access/>`__
     * `Instrument Paper <https://doi.org/10.1007/s11207-009-9487-6>`__
     """
     # Class attribute used to specify the source class of the TimeSeries.
     _source = 'eve'
     _url = "http://lasp.colorado.edu/home/eve/"
 
     @peek_show
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/fermi_gbm.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/goes.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/goes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides GOES XRS `~sunpy.timeseries.TimeSeries` source.
+This module provies GOES XRS `~sunpy.timeseries.TimeSeries` source.
 """
 from pathlib import Path
 from collections import OrderedDict
 
 import h5netcdf
 import numpy as np
 import packaging.version
@@ -118,15 +118,15 @@
         pattern_inst = ("GOES 1-{SatelliteNumber:02d} {}")
         pattern_new = ("sci_gxrs-l2-irrad_g{SatelliteNumber:02d}_d{year:4d}{month:2d}{day:2d}_{}.nc")
         pattern_old = ("go{SatelliteNumber:02d}{}{month:2d}{day:2d}.fits")
         pattern_r = ("sci_xrsf-l2-flx1s_g{SatelliteNumber:02d}_d{year:4d}{month:2d}{day:2d}_{}.nc")
         pattern_1m = ("sci_xrsf-l2-avg1m_g{SatelliteNumber:02d}_d{year:4d}{month:2d}{day:2d}_{}.nc")
         pattern_telescop = ("GOES {SatelliteNumber:02d}")
         # The ordering of where we get the metadata from is important.
-        # We always want to check ID first as that will most likely have the correct information.
+        # We alway want to check ID first as that will most likely have the correct information.
         # The other fields are fallback and sometimes have data in them that is "useless".
         id = (
             self.meta.metas[0].get("id", "").strip()
             or self.meta.metas[0].get("filename_id", "").strip()
             or self.meta.metas[0].get("TELESCOP", "").strip()
             or self.meta.metas[0].get("Instrument", "").strip()
         )
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/lyra.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/lyra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides Proba-2 `~sunpy.timeseries.TimeSeries` source.
+This module provies Proba-2 `~sunpy.timeseries.TimeSeries` source.
 """
 import sys
 from collections import OrderedDict
 
 import pandas
 
 import astropy.units as u
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/noaa.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/noaa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides NOAA Solar Cycle `~sunpy.timeseries.TimeSeries` source.
+This module provies NOAA Solar Cycle `~sunpy.timeseries.TimeSeries` source.
 """
 from pathlib import Path
 from collections import OrderedDict
 
 import numpy as np
 import pandas as pd
 
@@ -52,15 +52,15 @@
     * `Indices Descriptions <ftp://ftp.swpc.noaa.gov/pub/weekly/README3>`_
     * `NOAA plots of Solar Cycle Progression <https://www.swpc.noaa.gov/products/solar-cycle-progression>`_
     * `NOAA Product List <https://www.swpc.noaa.gov/products-and-data>`_
     """
     # Class attributes used to specify the source class of the TimeSeries
     # and a URL to the mission website.
     _source = 'noaaindices'
-    _url = "https://www.swpc.noaa.gov/products/solar-cycle-progression"
+    _url = "https://www.swpc.noaa.gov/products-and-data"
 
     def plot(self, axes=None, plot_type='sunspot SWO', columns=None, **kwargs):
         """
         Plots NOAA Indices.
 
         Parameters
         ----------
@@ -98,14 +98,16 @@
             ylabel = 'Geomagnetic AP Index'
         else:
             raise ValueError(f'Got unknown plot type "{type}"')
 
         to_plot = self.to_dataframe()[to_plot]
         to_plot.plot(ax=axes, **kwargs)
 
+        axes.set_xlim(min(to_plot.dropna(how='all').index),
+                      max(to_plot.dropna(how='all').index))
         axes.set_ylim(0)
         axes.set_ylabel(ylabel)
         axes.legend()
         self._setup_x_axis(axes)
         return axes
 
     @peek_show
@@ -224,15 +226,15 @@
     * `NOAA plots of Solar Cycle Progression <https://www.swpc.noaa.gov/products/solar-cycle-progression>`_
     * `NOAA Product List <https://www.swpc.noaa.gov/products-and-data>`_
     """
 
     # Class attributes used to specify the source class of the TimeSeries
     # and a URL to the mission website.
     _source = 'noaapredictindices'
-    _url = "https://www.swpc.noaa.gov/products/solar-cycle-progression"
+    _url = "https://www.swpc.noaa.gov/products-and-data"
 
     _peek_title = "Solar Cycle Sunspot Number Prediction"
 
     def plot(self, axes=None, columns=None, **plot_args):
         """
         Plots predicted NOAA Indices as a function of time from a pandas dataframe.
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/norh.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/norh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides a Nobeyama Radioheliograph `~sunpy.timeseries.TimeSeries`
+This module provies a Nobeyama Radioheliograph `~sunpy.timeseries.TimeSeries`
 source.
 """
 from collections import OrderedDict
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/rhessi.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/rhessi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides a RHESSI `~sunpy.timeseries.TimeSeries` source.
+This module provies a RHESSI `~sunpy.timeseries.TimeSeries` source.
 """
 import itertools
 from collections import OrderedDict
 
 import numpy as np
 from pandas import DataFrame
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/tests/test_eve.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_eve.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/tests/test_fermi_gbm.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/tests/test_goes.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_goes.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     assert isinstance(goes, sunpy.timeseries.sources.goes.XRSTimeSeries)
     # Newer format
     goes = sunpy.timeseries.TimeSeries(
         'https://umbra.nascom.nasa.gov/goes/fits/2018/go1520180626.fits')
     assert isinstance(goes, sunpy.timeseries.sources.goes.XRSTimeSeries)
     # Testing NOAA served data
     goes = sunpy.timeseries.TimeSeries(
-        'https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/goes16/l2/data/xrsf-l2-flx1s_science/2022/05/sci_xrsf-l2-flx1s_g16_d20220506_v2-2-0.nc')
+        'https://data.ngdc.noaa.gov/platforms/solar-space-observing-satellites/goes/goes16/l2/data/xrsf-l2-flx1s_science/2022/05/sci_xrsf-l2-flx1s_g16_d20220506_v2-1-0.nc')
     assert isinstance(goes, sunpy.timeseries.sources.goes.XRSTimeSeries)
 
 
 @figure_test
 def test_goes_peek(goes_test_ts):
     goes_test_ts.peek()
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/tests/test_lyra.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_lyra.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/tests/test_noaa.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_noaa.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/tests/test_norh.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_norh.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/sources/tests/test_rhessi.py` & `sunpy-4.1rc1/sunpy/timeseries/sources/tests/test_rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/tests/conftest.py` & `sunpy-4.1rc1/sunpy/timeseries/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/tests/test_timeseries_factory.py` & `sunpy-4.1rc1/sunpy/timeseries/tests/test_timeseries_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     assert ts.quantity('nH').unit == u.dimensionless_unscaled
 
     # Put back known unit registry, and check that units are recognised
     sunpy_cdf._known_units = known_units
     ts = sunpy.timeseries.TimeSeries(filename)
     assert ts.quantity('nH').unit == u.cm**-3
 
-    # Reset again to check that registering units via. astropy works too
+    # Reset again to check that registring units via. astropy works too
     sunpy_cdf._known_units = {}
     u.add_enabled_units([u.def_unit('#/cm^3', represents=u.cm**-3)])
     ts = sunpy.timeseries.TimeSeries(filename)
     assert ts.quantity('nH').unit == u.cm**-3
 
     sunpy_cdf._known_units = known_units
 
@@ -153,15 +153,15 @@
         ts_empty = sunpy.timeseries.TimeSeries(swa_filepath)
     assert ts_empty == []
     assert "No data found in file" in caplog.text
     assert "solo_L1_swa-pas-mom_20200706_V01.cdf" in caplog.text
 
 
 def test_meta_from_fits_header():
-    # Generate the data and the corresponding dates
+    # Generate the data and the corrisponding dates
     base = parse_time(datetime.datetime.today())
     times = base - TimeDelta(np.arange(24*60)*u.minute)
     intensity = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
     units = {'intensity': u.W/u.m**2}
     data = DataFrame(intensity, index=times, columns=['intensity'])
 
     # Use a FITS file HDU using sunpy.io
@@ -179,15 +179,15 @@
     meta_md = MetaDict(sunpy.io.header.FileHeader(meta))
     ts_hdu_meta = sunpy.timeseries.TimeSeries(data, meta, units)
     ts_md_meta = sunpy.timeseries.TimeSeries(data, meta_md, units)
     assert ts_hdu_meta == ts_md_meta
 
 
 def test_generic_construction_basic():
-    # Generate the data and the corresponding dates
+    # Generate the data and the corrisponding dates
     base = parse_time(datetime.datetime.today())
     times = base - TimeDelta(np.arange(24 * 60)*u.minute)
     intensity = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
 
     # Create the data DataFrame, header MetaDict and units OrderedDict
     data = DataFrame(intensity, index=times, columns=['intensity'])
     units = OrderedDict([('intensity', u.W/u.m**2)])
@@ -203,15 +203,15 @@
     # Create TS using a tuple of values
     ts_tuple = sunpy.timeseries.TimeSeries(((data, meta, units),))
     assert isinstance(ts_tuple, sunpy.timeseries.timeseriesbase.GenericTimeSeries)
     assert ts_generic == ts_tuple
 
 
 def test_generic_construction_basic_omitted_details():
-    # Generate the data and the corresponding dates
+    # Generate the data and the corrisponding dates
     base = parse_time(datetime.datetime.today())
     times = base - TimeDelta(np.arange(24 * 60)*u.minute)
     intensity = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
 
     # Create the data DataFrame, header MetaDict and units OrderedDict
     data = DataFrame(intensity, index=times, columns=['intensity'])
     units = OrderedDict([('intensity', u.W/u.m**2)])
@@ -229,15 +229,15 @@
     assert isinstance(ts_2, sunpy.timeseries.timeseriesbase.GenericTimeSeries)
     assert ts_2.columns == ['intensity']
     assert ts_2.units == units
     assert ts_2.meta.metadata[0][2] == MetaDict()
 
 
 def test_generic_construction_basic_different_meta_types():
-    # Generate the data and the corresponding dates
+    # Generate the data and the corrisponding dates
     base = parse_time(datetime.datetime.today())
     times = base - TimeDelta(np.arange(24 * 60)*u.minute)
     intensity = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
     tr = sunpy.time.TimeRange(times[0], times[-1])
 
     # Create the data DataFrame, header MetaDict and units OrderedDict
     data = DataFrame(intensity, index=times, columns=['intensity'])
@@ -254,15 +254,15 @@
     ts_od = sunpy.timeseries.TimeSeries(data, meta_od, units)
     ts_obj = sunpy.timeseries.TimeSeries(data, meta_obj, units)
     assert ts_md == ts_di == ts_od == ts_obj
     assert ts_md.meta.metadata[0][2] == ts_di.meta.metadata[0][2] == ts_od.meta.metadata[0][2] == ts_obj.meta.metadata[0][2]
 
 
 def test_generic_construction_ts_list():
-    # Generate the data and the corresponding dates
+    # Generate the data and the corrisponding dates
     base = parse_time(datetime.datetime.today())
     times = base - TimeDelta(np.arange(24 * 60)*u.minute)
     intensity1 = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
     intensity2 = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
 
     # Create the data DataFrame, header MetaDict and units OrderedDict
     data = DataFrame(intensity1, index=times, columns=['intensity'])
@@ -285,15 +285,15 @@
 
     # Create TS using a tuple
     ts_list2 = sunpy.timeseries.TimeSeries(((data, meta, units), (data2, meta2, units2)))
     assert ts_list == ts_list2
 
 
 def test_generic_construction_concatenation():
-    # Generate the data and the corresponding dates
+    # Generate the data and the corrisponding dates
     base = parse_time(datetime.datetime.today())
     times = base - TimeDelta(np.arange(24 * 60)*u.minute)
     intensity1 = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
     intensity2 = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (24*60))))
 
     # Create the data DataFrame, header MetaDict and units OrderedDict
     data = DataFrame(intensity1, index=times, columns=['intensity'])
@@ -304,15 +304,15 @@
     meta2 = MetaDict({'key2': 'value2'})
 
     # Create TS individually
     ts_1 = sunpy.timeseries.TimeSeries(data, meta, units)
     ts_2 = sunpy.timeseries.TimeSeries(data2, meta2, units2)
     ts_concat_1 = ts_1.concatenate(ts_2)
 
-    # Concatenate during construction
+    # Concatinate during construction
     ts_concat_2 = sunpy.timeseries.TimeSeries(
         data, meta, units, data2, meta2, units2, concatenate=True)
     assert isinstance(ts_concat_2, sunpy.timeseries.timeseriesbase.GenericTimeSeries)
 
     # Create TS using a tuple
     ts_concat_3 = sunpy.timeseries.TimeSeries(
         ((data, meta, units), (data2, meta2, units2)), concatenate=True)
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/tests/test_timeseriesbase.py` & `sunpy-4.1rc1/sunpy/timeseries/tests/test_timeseriesbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,15 @@
     with pytest.raises(TypeError, match="TimeSeries classes must match if "
                                         "'same_source' is specified."):
         eve_test_ts.concatenate(fermi_gbm_test_ts, same_source=True)
 
 
 def test_generic_construction_concatenation():
     nrows = 10
-    # Generate the data and the corresponding dates
+    # Generate the data and the corrisponding dates
     base = parse_time(datetime.datetime.today())
     times = base - TimeDelta(np.arange(nrows)*u.minute)
     intensity1 = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (nrows))))
     intensity2 = np.sin(np.arange(0, 12 * np.pi, ((12 * np.pi) / (nrows))))
 
     # Create the data DataFrame, header MetaDict and units OrderedDict
     data = DataFrame(intensity1, index=times, columns=['intensity'])
@@ -396,15 +396,15 @@
              np.isnan(column_quantity.value))).all()
 
 
 def test_add_column_from_quantity(eve_test_ts, column_quantity):
     new_ts = eve_test_ts.add_column('quantity_added', column_quantity)
     # Test the column similar to the original quantity?
     assert_quantity_allclose(new_ts.quantity('quantity_added'), column_quantity)
-    # Test the full list of columns are present
+    # Test the full list of columns are pressent
     assert set(new_ts.to_dataframe().columns) == set(
         eve_test_ts.to_dataframe().columns) | {'quantity_added'}
 
 
 def test_remove_column(eve_test_ts):
     removed = eve_test_ts.remove_column('XRS-B proxy')
     # Check that column remains in eve_test_ts but isn't in removed
@@ -414,27 +414,27 @@
 
     # Check units updated correctly
     assert len(removed.columns) == len(removed.units)
 
     # Check data updated correctly
     assert len(removed.columns) == removed.to_dataframe().shape[1]
 
-    # Check that removing a non-existent column errors
+    # Check that removing a non-existant column errors
     with pytest.raises(ValueError):
         eve_test_ts.remove_column('random column name')
 
 
 def test_add_column_from_array(eve_test_ts, column_quantity):
     # Test the column similar to the original quantity?
     new_ts = eve_test_ts.add_column(
         'array_added', column_quantity.value, unit=column_quantity.unit)
     assert_quantity_allclose(
         new_ts.quantity('array_added'), column_quantity)
 
-    # Test the full list of columns are present
+    # Test the full list of columns are pressent
     assert set(new_ts.to_dataframe().columns) == set(
         eve_test_ts.to_dataframe().columns) | {'array_added'}
 
 
 def test_add_column_from_array_no_units(eve_test_ts, column_quantity):
     ts = eve_test_ts.add_column('array_added', column_quantity.value)
     assert (ts.quantity('array_added') == column_quantity.value).all()
@@ -485,15 +485,15 @@
     assert generic_ts == generic_copy_ts
     generic_copy_ts.meta.metadata[0][2]['key'] = 1
     assert generic_ts != generic_copy_ts
     assert generic_ts != table_ts
 
 
 def test_equality_different_ts_types(generic_ts, eve_test_ts):
-    # this should fail as they're not the same type and can't match
+    # this should fail as they're not the smae type and can't match
     assert not (generic_ts == eve_test_ts)
 
 
 def test_ts_index(generic_ts):
     with pytest.warns(SunpyDeprecationWarning, match='.index is deprecatd'):
         assert (generic_ts.index == generic_ts.to_dataframe().index).all()
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/tests/test_timeseriesmetadata.py` & `sunpy-4.1rc1/sunpy/timeseries/tests/test_timeseriesmetadata.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/timeseries/timeseries_factory.py` & `sunpy-4.1rc1/sunpy/timeseries/timeseries_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides the `~sunpy.timeseries.TimeSeriesFactory` class.
+This module provies the `~sunpy.timeseries.TimeSeriesFactory` class.
 """
 import os
 import copy
 import pathlib
 from collections import OrderedDict
 from urllib.request import Request
```

### Comparing `sunpy-4.1.5/sunpy/timeseries/timeseriesbase.py` & `sunpy-4.1rc1/sunpy/timeseries/timeseriesbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provides `sunpy.timeseries.GenericTimeSeries` which all other
+This module provies `sunpy.timeseries.GenericTimeSeries` which all other
 `sunpy.timeseries.TimeSeries` classes inherit from.
 """
 import copy
 import html
 import time
 import textwrap
 import webbrowser
@@ -347,15 +347,15 @@
                     dat[self.columns[i]].values[~np.isnan(dat[self.columns[i]].values)],
                     log=True,
                     bins="scott",
                     color=cols[i],
                 )
                 plt.title(self.columns[i] + " [click for other channels]")
                 plt.xlabel(self.units[self.columns[i]])
-                plt.ylabel("# of occurrences")
+                plt.ylabel("# of occurences")
                 hlist.append(_figure_to_base64(fig))
                 plt.close(fig)
 
         # This loop creates a formatted list of base64 images that is passed
         # directly into the JS script below, so all images are written into
         # the html page when it is created (allows for an arbitrary number of
         # histograms to be rotated through onclick).
@@ -853,15 +853,15 @@
         * Remove entries outside of the dates or truncate if the metadata overflows past the data.
         * Remove column references in the metadata that don't match to a column in the data.
         * Remove metadata entries that have no columns matching the data.
         """
         # Truncate the metadata
         self.meta._truncate(self.time_range)
 
-        # Remove non-existent columns
+        # Remove non-existant columns
         redundant_cols = list(set(self.meta.columns) - set(self.columns))
         self.meta._remove_columns(redundant_cols)
 
 # #### Export/Output Methods #### #
 
     def to_table(self, **kwargs):
         """
```

### Comparing `sunpy-4.1.5/sunpy/util/config.py` & `sunpy-4.1rc1/sunpy/util/config.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/datatype_factory_base.py` & `sunpy-4.1rc1/sunpy/util/datatype_factory_base.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/decorators.py` & `sunpy-4.1rc1/sunpy/util/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
             instance
                 Any class instance that has the property ``prop``,
                 and attribute ``attr``.
             """
             cache = instance.__dict__
             prop_key = prop.__name__
 
-            # Check if our caching method has changed output
+            # Check if our caching method has changed ouptut
             new_attr_val = getattr(instance, attr_name)
             old_attr_val = cache.get(attr_name, _NOT_FOUND)
             if (old_attr_val is _NOT_FOUND or
                     new_attr_val != old_attr_val or
                     prop_key not in cache):
                 # Store the new attribute value
                 cache[attr_name] = new_attr_val
```

### Comparing `sunpy-4.1.5/sunpy/util/exceptions.py` & `sunpy-4.1rc1/sunpy/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/functools.py` & `sunpy-4.1rc1/sunpy/util/functools.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/io.py` & `sunpy-4.1rc1/sunpy/util/io.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/logger.py` & `sunpy-4.1rc1/sunpy/util/logger.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/metadata.py` & `sunpy-4.1rc1/sunpy/util/metadata.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/net.py` & `sunpy-4.1rc1/sunpy/util/net.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/parfive_helpers.py` & `sunpy-4.1rc1/sunpy/util/parfive_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 parfive_version = Version(parfive.__version__)
 sunpy_headers = {
     "User-Agent": f"sunpy/{sunpy.__version__} parfive/{parfive.__version__} "
     f"aiohttp/{aiohttp.__version__} python/{sys.version[:5]}"
 }
 
 
-if parfive_version < Version("2.0.0"):
+if parfive_version < Version("2.0a0"):
     # Overload the parfive downloader class to set the User-Agent string
     class Downloader(parfive.Downloader):
         @wraps(parfive.Downloader.__init__)
         def __init__(self, *args, **kwargs):
             headers = kwargs.pop("headers", {})
             kwargs["headers"] = {**sunpy_headers, **headers}
+
             # Works with conftest to hide the progress bar.
             progress = os.environ.get("PARFIVE_HIDE_PROGESS", None)
             if progress:
                 kwargs["progress"] = False
+
             super().__init__(*args, **kwargs)
 
 else:
     from parfive import SessionConfig
 
     config = SessionConfig(headers=sunpy_headers)
 
@@ -42,8 +44,9 @@
             if "config" not in kwargs:
                 kwargs["config"] = config
 
             # This is to make our sample data download code work on 1.x and 2.x
             # when we depend on 2+ we should remove this.
             headers = kwargs.pop("headers", {})
             kwargs["config"].headers = {**kwargs["config"].headers, **headers}
+
             super().__init__(*args, **kwargs)
```

### Comparing `sunpy-4.1.5/sunpy/util/sphinx/__init__.py` & `sunpy-4.1rc1/sunpy/util/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/sphinx/doctest.py` & `sunpy-4.1rc1/sunpy/util/sphinx/doctest.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/sphinx/generate.py` & `sunpy-4.1rc1/sunpy/util/sphinx/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         attributes = {'format': ' '.join(self.arguments[0].lower().split())}
 
         source, lineno = self.state_machine.get_source_and_line(self.lineno)
 
         old_stdout, sys.stdout = sys.stdout, StringIO()
         try:
-            # Execute the Python code and capture its output
+            # Exceute the Python code and capture its output
             exec('\n'.join(self.content))
             text = sys.stdout.getvalue()
 
             # Wrap HTML output in a black border if requested
             if attributes['format'] == 'html' and 'html_border' in self.options:
                 text = f"<div style='border:1px solid black; padding:3px'>{text}</div>"
```

### Comparing `sunpy-4.1.5/sunpy/util/sysinfo.py` & `sunpy-4.1rc1/sunpy/util/sysinfo.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_config.py` & `sunpy-4.1rc1/sunpy/util/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_datatype_factory_base.py` & `sunpy-4.1rc1/sunpy/util/tests/test_datatype_factory_base.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_decorators.py` & `sunpy-4.1rc1/sunpy/util/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_functools.py` & `sunpy-4.1rc1/sunpy/util/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_logger.py` & `sunpy-4.1rc1/sunpy/util/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_metadata.py` & `sunpy-4.1rc1/sunpy/util/tests/test_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
 
 #  Test `MetaDict.update(...)`.
 
 
 def test_update_with_distinct_keys(seas_metadict, sea_locations, atomic_weights):
     """
     Update the MetaDict 'world_seas', with another MetaDict, 'chem_elems' which
-    has a completely different set of keys.
+    has a completley different set of keys.
 
     This should result in adding 'chem_elems' onto 'world_seas'.
     Original insertion order of 'world_seas' should be preserved.
     """
     world_seas = seas_metadict
     chem_elems = MetaDict(atomic_weights)
     world_seas.update(chem_elems)
```

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_net.py` & `sunpy-4.1rc1/sunpy/util/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_sysinfo.py` & `sunpy-4.1rc1/sunpy/util/tests/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_util.py` & `sunpy-4.1rc1/sunpy/util/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/util/tests/test_xml.py` & `sunpy-4.1rc1/sunpy/util/tests/test_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
     assert len(expected['Config']) == len(actual['Config'])
     assert expected['Config']['Name'] == actual['Config']['Name']
 
     assert len(actual['Config']['Children']) == 2
 
     # As the child dictionaries are in lists we cannot be certain what order
-    # they are in. Test individually.
+    # they are in. Test individualy.
 
     expected_children = expected['Config']['Children']
     actual_children = actual['Config']['Children']
 
     expected_first_child = getChild(expected_children, key='Name', value='First Child')
     actual_first_child = getChild(actual_children, key='Name', value='First Child')
```

### Comparing `sunpy-4.1.5/sunpy/util/util.py` & `sunpy-4.1rc1/sunpy/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     Makes sure that a list of dictionaries all have the same keys.
 
     If a key is missing, it will be added but with a value of None.
 
     Parameters
     ----------
     list_of_dicts : `list` of `dict`
-          A list containing each dictionary to parse.
+          A list containing each dictonary to parse.
 
     Returns
     ------
     `list`
         The list with each dict updated.
 
     References
```

### Comparing `sunpy-4.1.5/sunpy/util/xml.py` & `sunpy-4.1rc1/sunpy/util/xml.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/version.py` & `sunpy-4.1rc1/sunpy/version.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/animator/mapsequenceanimator.py` & `sunpy-4.1rc1/sunpy/visualization/animator/mapsequenceanimator.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/animator/tests/test_mapsequenceanimator.py` & `sunpy-4.1rc1/sunpy/visualization/animator/tests/test_mapsequenceanimator.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/cm.py` & `sunpy-4.1rc1/sunpy/visualization/colormaps/cm.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/color_tables.py` & `sunpy-4.1rc1/sunpy/visualization/colormaps/color_tables.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_dark_blue.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_dark_blue.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_dark_green.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_dark_green.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_dark_red.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_dark_red.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/eit_yellow.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/eit_yellow.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_171.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_171.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_195.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_195.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_284.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_284.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/euvi_304.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/euvi_304.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/grayscale.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/grayscale.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/hi1.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/hi1.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/hi2.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/hi2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/hmi_mag.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/hmi_mag.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/idl_3.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/idl_3.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/lasco_c2.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/lasco_c2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/lasco_c3.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/lasco_c3.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/rhessi.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/rhessi.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/std_gamma_2.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/std_gamma_2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/stereo_cor1.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/stereo_cor1.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/stereo_cor2.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/stereo_cor2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1216.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1216.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1550.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1550.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1600.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1600.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_1700.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_1700.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_171.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_171.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_195.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_195.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/data/trace_284.csv` & `sunpy-4.1rc1/sunpy/visualization/colormaps/data/trace_284.csv`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/colormaps/tests/test_cm.py` & `sunpy-4.1rc1/sunpy/visualization/colormaps/tests/test_cm.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/drawing.py` & `sunpy-4.1rc1/sunpy/visualization/drawing.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/limb.py` & `sunpy-4.1rc1/sunpy/visualization/limb.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/tests/test_drawing.py` & `sunpy-4.1rc1/sunpy/visualization/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/visualization.py` & `sunpy-4.1rc1/sunpy/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy/visualization/wcsaxes_compat.py` & `sunpy-4.1rc1/sunpy/visualization/wcsaxes_compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 This module provides functions to make WCSAxes work in SunPy.
 """
 import matplotlib.pyplot as plt
-from packaging.version import Version
 
 import astropy.units as u
-from astropy import __version__ as astropy_version
 from astropy.visualization import wcsaxes
 
 from sunpy.coordinates import HeliographicCarrington, HeliographicStonyhurst
 
 __all__ = ["is_wcsaxes", "gca_wcs", "get_world_transform",
            "default_wcs_grid", "wcsaxes_heliographic_overlay"]
 
@@ -170,19 +168,15 @@
     c1, c2 = axes.coords
     c1.set_ticks_position('bl')
     c2.set_ticks_position('bl')
 
     lon = overlay[0]
     lat = overlay[1]
 
-    # TODO: Remove when we depend on astropy 5.3
-    if Version(astropy_version) >= Version("5.3.dev"):
-        lon.coord_wrap = 180 * u.deg
-    else:
-        lon.coord_wrap = 180
+    lon.coord_wrap = 180
     lon.set_major_formatter('dd')
 
     if annotate:
         lon.set_axislabel(f'{system.capitalize()} Longitude', minpad=0.8)
         lat.set_axislabel(f'{system.capitalize()} Latitude', minpad=0.9)
         lon.set_ticks_position('tr')
         lat.set_ticks_position('tr')
```

### Comparing `sunpy-4.1.5/sunpy-dev-env.yml` & `sunpy-4.1rc1/sunpy-dev-env.yml`

 * *Files identical despite different names*

### Comparing `sunpy-4.1.5/sunpy.egg-info/PKG-INFO` & `sunpy-4.1rc1/sunpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy
-Version: 4.1.5
+Version: 4.1rc1
 Summary: SunPy core package: Python for Solar Physics
 Home-page: https://sunpy.org
 Download-URL: https://pypi.org/project/sunpy/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/sunpy/
@@ -50,15 +50,15 @@
 |Latest Version| |DOI| |matrix| |codecov| |Binder| |Powered by NumFOCUS|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/sunpy.svg
    :target: https://pypi.python.org/pypi/sunpy/
 .. |DOI| image:: https://zenodo.org/badge/2165383.svg
    :target: https://zenodo.org/badge/latestdoi/2165383
 .. |matrix| image:: https://img.shields.io/matrix/sunpy:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=openastronomy.modular.im
-   :target: https://app.element.io/#/room/#sunpy:openastronomy.org
+   :target: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
 .. |codecov| image:: https://codecov.io/gh/sunpy/sunpy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/sunpy/sunpy/main?filepath=examples
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
 
@@ -120,8 +120,8 @@
 This will walk you through getting set up for contributing.
 
 Code of Conduct
 ===============
 
 When you are interacting with the SunPy community you are asked to follow our `Code of Conduct <https://sunpy.org/coc>`__.
 
-.. _SunPy Chat: https://app.element.io/#/room/#sunpy:openastronomy.org
+.. _SunPy Chat: https://openastronomy.element.io/#/room/#sunpy:openastronomy.org
```

### Comparing `sunpy-4.1.5/sunpy.egg-info/SOURCES.txt` & `sunpy-4.1rc1/sunpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,14 @@
 examples/map_transformations/projection_custom_origin.py
 examples/map_transformations/reprojection_aia_euvi_mosaic.py
 examples/map_transformations/reprojection_align_aia_hmi.py
 examples/map_transformations/reprojection_carrington.py
 examples/map_transformations/reprojection_different_observers.py
 examples/map_transformations/reprojection_spherical_screen.py
 examples/map_transformations/upside_down_hmi.py
-examples/plotting/AIA_HMI_composite.py
 examples/plotting/README.txt
 examples/plotting/aia_example.py
 examples/plotting/arrayanimatorwcs.py
 examples/plotting/fading_between_maps.py
 examples/plotting/finding_local_peaks_in_solar_data.py
 examples/plotting/finegrained_plot.py
 examples/plotting/great_arc_example.py
@@ -161,25 +160,22 @@
 examples/plotting/hmi_cutout.py
 examples/plotting/hmi_synoptic_maps.py
 examples/plotting/lat_lon_lines.py
 examples/plotting/limb_plotting.py
 examples/plotting/lineAnimator_examples.py
 examples/plotting/magnetogram_active_regions.py
 examples/plotting/map_editcolormap.py
-examples/plotting/masked_composite_plot.py
 examples/plotting/overplot_hek_polygon.py
 examples/plotting/plot_equator_prime_meridian.py
 examples/plotting/plot_rectangle.py
 examples/plotting/plotting_blank_map.py
 examples/plotting/quadrangle.py
-examples/plotting/rgb_composite.py
 examples/plotting/simple_differential_rotation.py
 examples/plotting/solar_cycle_example.py
 examples/plotting/sunpy_matplotlib_colormap.py
-examples/plotting/three_map_composite.py
 examples/plotting/wcsaxes_map_example.py
 examples/plotting/wcsaxes_plotting_example.py
 examples/plotting/xy_lims.py
 examples/saving_and_loading_data/README.txt
 examples/saving_and_loading_data/coordinates_in_asdf.py
 examples/saving_and_loading_data/genericmap_in_asdf.py
 examples/saving_and_loading_data/genericmap_in_fits.py
@@ -255,25 +251,23 @@
 sunpy/data/data_manager/manager.py
 sunpy/data/data_manager/storage.py
 sunpy/data/data_manager/tests/__init__.py
 sunpy/data/data_manager/tests/conftest.py
 sunpy/data/data_manager/tests/db_testdata.csv
 sunpy/data/data_manager/tests/mocks.py
 sunpy/data/data_manager/tests/test_cache.py
-sunpy/data/data_manager/tests/test_downloader.py
 sunpy/data/data_manager/tests/test_manager.py
 sunpy/data/data_manager/tests/test_storage.py
 sunpy/data/test/20100621SRS.txt
 sunpy/data/test/2013_05_13__16_54_06_137__SOHO_LASCO_C3_white-light.jp2
 sunpy/data/test/2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2
 sunpy/data/test/20150101SRS.txt
 sunpy/data/test/20150306SRS.txt
 sunpy/data/test/20150906SRS.txt
 sunpy/data/test/20181209_180305_kcor_l2.header
-sunpy/data/test/2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2
 sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt
 sunpy/data/test/FGMG4_20110214_030443.7.header
 sunpy/data/test/HinodeSOT.header
 sunpy/data/test/HinodeXRT.header
 sunpy/data/test/YohkohSXT.header
 sunpy/data/test/__init__.py
 sunpy/data/test/_generate_asdf_test.py
@@ -286,15 +280,14 @@
 sunpy/data/test/euvi_20090615_000900_n4euA_s.header
 sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits
 sunpy/data/test/gbm.fits
 sunpy/data/test/generated_sample.genx
 sunpy/data/test/go1520110607.fits
 sunpy/data/test/go1520120601.fits.gz
 sunpy/data/test/goes_13_leap_second.nc
-sunpy/data/test/gzip_fits_test.file
 sunpy/data/test/gzip_test.fit.gz
 sunpy/data/test/gzip_test.fits.gz
 sunpy/data/test/gzip_test.fts.gz
 sunpy/data/test/heliographic_phase_map.fits.gz
 sunpy/data/test/hi_20110910_114721_s7h2A.header
 sunpy/data/test/hmi_synoptic.header
 sunpy/data/test/hsi_image_20101016_191218.fits
@@ -311,15 +304,14 @@
 sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
 sunpy/data/test/resampled_hmi.fits
 sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc
 sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc
 sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc
 sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc
 sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc
-sunpy/data/test/seit_00171_fd_19961211_1900.header
 sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header
 sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf
 sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf
 sunpy/data/test/swap_lv1_20140606_000113.header
 sunpy/data/test/tca110810_truncated
 sunpy/data/test/test_ana.fz
 sunpy/data/test/tsi20010130_025823_a2.header
```

### Comparing `sunpy-4.1.5/sunpy.egg-info/requires.txt` & `sunpy-4.1rc1/sunpy.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [all]
 asdf-astropy>=0.1.1
 asdf>=2.8.0
 dask[array]>=2.0.0
 sqlalchemy>=1.3.4
 scikit-image>=0.16.0
-scipy!=1.10.0,>=1.3.0
+scipy>=1.3.0
 glymur!=0.9.0,!=0.9.5,>=0.8.18
 lxml>=4.8.0
 matplotlib>=3.3.0
 mpl-animators>=1.0.0
 reproject
 beautifulsoup4>=4.8.0
 drms>=0.6.1
@@ -37,15 +37,15 @@
 
 [dev]
 asdf-astropy>=0.1.1
 asdf>=2.8.0
 dask[array]>=2.0.0
 sqlalchemy>=1.3.4
 scikit-image>=0.16.0
-scipy!=1.10.0,>=1.3.0
+scipy>=1.3.0
 glymur!=0.9.0,!=0.9.5,>=0.8.18
 lxml>=4.8.0
 matplotlib>=3.3.0
 mpl-animators>=1.0.0
 reproject
 beautifulsoup4>=4.8.0
 drms>=0.6.1
@@ -70,52 +70,48 @@
 packaging
 ruamel.yaml
 sphinx
 sphinx-automodapi
 sphinx-changelog>=1.1.1
 sphinx-copybutton
 sphinx-design
-sphinx-gallery>=0.11.1
+sphinx-gallery>=0.9.0
 sphinxext-opengraph
-sunkit_image
 sunpy-sphinx-theme
-towncrier<22.12.0
 
 [docs]
 astroquery
 hvpy>=1.0.1
 jplephem
 opencv-python
 packaging
 reproject
 ruamel.yaml
 sphinx
 sphinx-automodapi
 sphinx-changelog>=1.1.1
 sphinx-copybutton
 sphinx-design
-sphinx-gallery>=0.11.1
+sphinx-gallery>=0.9.0
 sphinxext-opengraph
-sunkit_image
 sunpy-sphinx-theme
-towncrier<22.12.0
 
 [image]
 scikit-image>=0.16.0
-scipy!=1.10.0,>=1.3.0
+scipy>=1.3.0
 
 [jpeg2000]
 glymur!=0.9.0,!=0.9.5,>=0.8.18
 lxml>=4.8.0
 
 [map]
 matplotlib>=3.3.0
 mpl-animators>=1.0.0
 reproject
-scipy!=1.10.0,>=1.3.0
+scipy>=1.3.0
 
 [net]
 beautifulsoup4>=4.8.0
 drms>=0.6.1
 python-dateutil>=2.8.0
 tqdm>=4.32.1
 zeep>=3.4.0
```

### Comparing `sunpy-4.1.5/tox.ini` & `sunpy-4.1rc1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     hypothesis: using hypothesis (both offline and online)
     figure: runs the figure test suite.
 setenv =
     MPLBACKEND = agg
     SUNPY_SAMPLEDIR = {env:SUNPY_SAMPLEDIR:{toxinidir}/.tox/sample_data/}
     PYTEST_COMMAND = pytest -vvv -r a --pyargs sunpy --cov-report=xml --cov=sunpy --cov-config={toxinidir}/setup.cfg {toxinidir}/docs
     devdeps,build_docs,online: HOME = {envtmpdir}
-    PARFIVE_HIDE_PROGRESS = True
+    HIDE_PARFIVE_PROGESS = True
     NO_VERIFY_HELIO_SSL = 1
     devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/astropy/simple https://pypi.anaconda.org/scipy-wheels-nightly/simple
 deps =
     # devdeps is intended to be used to install the latest developer version of key dependencies.
     devdeps: astropy>=0.0.dev0
     devdeps: matplotlib>=0.0.dev0
     devdeps: git+https://github.com/asdf-format/asdf
@@ -43,15 +43,15 @@
     # Oldest deps we pin against
     oldestdeps: astropy<4.3.0
     oldestdeps: numpy<1.18.0
     oldestdeps: parfive<1.3.0
     oldestdeps: asdf<2.9.0
     oldestdeps: asdf-astropy<0.1.2
     oldestdeps: dask[array]<2.1.0
-    oldestdeps: sqlalchemy<2.0.0
+    oldestdeps: sqlalchemy<1.4.0
     oldestdeps: matplotlib<3.4.0
     oldestdeps: pandas<1.1.0
     oldestdeps: scipy<1.4.0
     oldestdeps: scikit-image<0.17.0
     oldestdeps: glymur<0.9.0
     oldestdeps: beautifulsoup4<4.9.0
     oldestdeps: drms<0.7
@@ -67,15 +67,14 @@
     online: pytest-timeout
     online: astroquery
     hypothesis: astroquery
     # Figure tests need a tightly controlled environment
     figure-!devdeps: astropy==5.1.0
     figure-!devdeps: matplotlib==3.5.2
     figure-!devdeps: mpl-animators==1.0.0
-    figure-!devdeps: numpy<1.24
 extras =
     all
     tests
 commands =
     pip freeze --all --no-input
     oldestdeps: python -c "import astropy.time; astropy.time.update_leap_seconds()"
     !online-!hypothesis-!figure: {env:PYTEST_COMMAND} {posargs}
@@ -121,14 +120,17 @@
 
 # Requires tox-conda
 [testenv:py{38,39,310}-conda]
 pypi_filter =
 extras =
 deps =
 conda_env = sunpy-dev-env.yml
+conda_deps =
+    pytest<7.2
+    pytest-xdist<3.0
 conda_channels = conda-forge
 install_command = pip install --no-deps --no-build-isolation {opts} {packages}
 allowlist_externals = conda
 commands_pre =
 #   Remove pytest-rerunfailures to avoid appearing to access the internet when pytest-xdist is used
     conda remove -y -q --force pytest-rerunfailures
 commands =
```

