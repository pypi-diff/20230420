# Comparing `tmp/sleplet-1.3.6.tar.gz` & `tmp/sleplet-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleplet-1.3.6.tar", last modified: Mon Apr 17 09:42:23 2023, max compression
+gzip compressed data, was "sleplet-1.4.0.tar", last modified: Thu Apr 20 16:42:51 2023, max compression
```

## Comparing `sleplet-1.3.6.tar` & `sleplet-1.4.0.tar`

### file list

```diff
@@ -1,209 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.874808 sleplet-1.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.834807 sleplet-1.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/ISSUE_TEMPLATE/question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/licence.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/paper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 09:42:10.000000 sleplet-1.3.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 09:42:10.000000 sleplet-1.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 09:42:10.000000 sleplet-1.3.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 09:42:10.000000 sleplet-1.3.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-17 09:42:10.000000 sleplet-1.3.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 09:42:10.000000 sleplet-1.3.6/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-17 09:42:23.874808 sleplet-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-17 09:42:10.000000 sleplet-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/DOCUMENTATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/config.mako
--rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-04-17 09:42:10.000000 sleplet-1.3.6/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.834807 sleplet-1.3.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/examples/arbitrary/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/_denoising_slepian_wavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/_slepian_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.838807 sleplet-1.3.6/examples/arbitrary/africa/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/denoising_slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/eigenvalues_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/slepian_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/tiling_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/africa/wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/eigenvalues_combined.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/arbitrary/south_america/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/eigenvalues_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/tiling_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/denoising_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/mesh_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/mesh_slepian_eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/mesh_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/mesh/produce_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/_denoising_axisym.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/denoising_axisym_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/denoising_axisym_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/denoising_axisym_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/translation_normalisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/misc/wavelet_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/polar_cap/
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/eigenfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/fried_egg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/simons_5_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/simons_5_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/polar_cap/slepian_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/examples/wavelets/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/wavelets/axisymmetric_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-17 09:42:10.000000 sleplet-1.3.6/examples/wavelets/axisymmetric_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.842807 sleplet-1.3.6/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-17 09:42:10.000000 sleplet-1.3.6/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-17 09:42:10.000000 sleplet-1.3.6/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-17 09:42:10.000000 sleplet-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:42:23.874808 sleplet-1.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.834807 sleplet-1.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.846807 sleplet-1.3.6/src/sleplet/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_array_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_bool_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_class_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_convolution_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.850808 sleplet-1.3.6/src/sleplet/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/create_earth_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/create_wmap_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_bird.off
--rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cheetah.off
--rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cube.off
--rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_dragon.off
--rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_homer.off
--rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_polygons_teapot.off
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_bird.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_cheetah.toml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_cube.toml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_dragon.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_homer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/meshes_regions_teapot.toml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_data/setup_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_mask_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_mesh_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_parallel_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_plotly_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.854807 sleplet-1.3.6/src/sleplet/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_scripts/plotting_on_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_scripts/plotting_on_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_slepian_arbitrary_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_string_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.862808 sleplet-1.3.6/src/sleplet/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/directional_spin_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/elongated_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/harmonic_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/noise_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/ridgelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_noise_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_noise_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/spherical_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/squashed_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/functions/wmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/harmonic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.866808 sleplet-1.3.6/src/sleplet/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/_mesh_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_harmonic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plot_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.866808 sleplet-1.3.6/src/sleplet/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plotting/_create_plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/plotting/_create_plot_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.870808 sleplet-1.3.6/src/sleplet/slepian/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_limit_lat_lon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian/slepian_polar_cap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/slepian_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-17 09:42:10.000000 sleplet-1.3.6/src/sleplet/wavelet_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.846807 sleplet-1.3.6/src/sleplet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 09:42:23.000000 sleplet-1.3.6/src/sleplet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:42:23.874808 sleplet-1.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_arbitrary_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_loading_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-17 09:42:10.000000 sleplet-1.3.6/tests/test_wavelets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.982827 sleplet-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.950825 sleplet-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.954825 sleplet-1.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/ISSUE_TEMPLATE/question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.954825 sleplet-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/licence.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/paper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 16:42:35.000000 sleplet-1.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 16:42:35.000000 sleplet-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 16:42:35.000000 sleplet-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-20 16:42:35.000000 sleplet-1.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-20 16:42:35.000000 sleplet-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-20 16:42:35.000000 sleplet-1.4.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-20 16:42:51.982827 sleplet-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-20 16:42:35.000000 sleplet-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/DOCUMENTATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/config.mako
+-rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-04-20 16:42:35.000000 sleplet-1.4.0/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.950825 sleplet-1.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/examples/arbitrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/_denoising_slepian_wavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/_slepian_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/examples/arbitrary/africa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/denoising_slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/eigenvalues_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/slepian_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/tiling_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/africa/wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/eigenvalues_combined.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.958826 sleplet-1.4.0/examples/arbitrary/south_america/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/eigenvalues_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/tiling_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/denoising_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/mesh_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/mesh_slepian_eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/mesh_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/mesh/produce_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/_denoising_axisym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/denoising_axisym_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/denoising_axisym_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/denoising_axisym_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/translation_normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/misc/wavelet_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/polar_cap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/eigenfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/fried_egg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/simons_5_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/simons_5_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/polar_cap/slepian_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/examples/wavelets/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/wavelets/axisymmetric_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-20 16:42:35.000000 sleplet-1.4.0/examples/wavelets/axisymmetric_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.962826 sleplet-1.4.0/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-04-20 16:42:35.000000 sleplet-1.4.0/paper/arxiv.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-20 16:42:35.000000 sleplet-1.4.0/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-20 16:42:35.000000 sleplet-1.4.0/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-20 16:42:35.000000 sleplet-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:42:51.982827 sleplet-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.950825 sleplet-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.966826 sleplet-1.4.0/src/sleplet/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_array_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_bool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_class_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_convolution_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.970827 sleplet-1.4.0/src/sleplet/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/create_earth_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/create_wmap_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_bird.off
+-rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cheetah.off
+-rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cube.off
+-rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_dragon.off
+-rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_homer.off
+-rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_polygons_teapot.off
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_bird.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_cheetah.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_cube.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_dragon.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_homer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/meshes_regions_teapot.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_data/setup_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_mask_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_mesh_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_parallel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_plotly_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.970827 sleplet-1.4.0/src/sleplet/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_scripts/plotting_on_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_scripts/plotting_on_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_slepian_arbitrary_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_string_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.974827 sleplet-1.4.0/src/sleplet/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/directional_spin_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/elongated_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/harmonic_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/noise_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/ridgelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_noise_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_noise_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/spherical_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/squashed_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/functions/wmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/harmonic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.978827 sleplet-1.4.0/src/sleplet/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/_mesh_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_harmonic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plot_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.978827 sleplet-1.4.0/src/sleplet/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plotting/_create_plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/plotting/_create_plot_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.982827 sleplet-1.4.0/src/sleplet/slepian/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_limit_lat_lon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian/slepian_polar_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/slepian_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-20 16:42:35.000000 sleplet-1.4.0/src/sleplet/wavelet_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.970827 sleplet-1.4.0/src/sleplet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 16:42:51.000000 sleplet-1.4.0/src/sleplet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:42:51.982827 sleplet-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_arbitrary_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_loading_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-20 16:42:35.000000 sleplet-1.4.0/tests/test_wavelets.py
```

### Comparing `sleplet-1.3.6/.github/ISSUE_TEMPLATE/bug_report.md` & `sleplet-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/.github/ISSUE_TEMPLATE/feature_request.md` & `sleplet-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/.github/workflows/deploy.yml` & `sleplet-1.4.0/.github/workflows/deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install build
+        run: python -m pip install build
 
       - name: Build distributions
         run: python -m build
 
       - name: Publish package to TestPyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `sleplet-1.3.6/.github/workflows/documentation.yml` & `sleplet-1.4.0/.github/workflows/documentation.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install -e .[docs]
+        run: python -m pip install -e .[docs]
 
       - name: Create documentation
         run: pdoc --html src/sleplet --template-dir documentation
 
       - name: Deploy
         uses: peaceiris/actions-gh-pages@v3
         with:
```

### Comparing `sleplet-1.3.6/.github/workflows/examples.yml` & `sleplet-1.4.0/.github/workflows/examples.yml`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,19 @@
           python-version: "3.10"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Cache pooch
         uses: actions/cache@v3
         with:
-          path: |
-            ~/.cache/sleplet
+          path: ~/.cache/sleplet
           key: readme-${{ hashFiles('pyproject.toml') }}
 
       - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install -e .[readme]
+        run: python -m pip install -e .[readme]
 
       - name: Run examples in the README
         run: python -m pytest --codeblocks .github README.md documentation
 
   examples:
     runs-on: ubuntu-latest
     steps:
@@ -44,23 +41,20 @@
           python-version: "3.10"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Cache pooch
         uses: actions/cache@v3
         with:
-          path: |
-            ~/.cache/sleplet
+          path: ~/.cache/sleplet
           key: examples-${{ hashFiles('pyproject.toml') }}
 
       - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install -e .[docs]
+        run: python -m pip install -e .[docs]
 
       - name: Run examples in the examples folder
-        run: |
-          find examples -name "*.py" \
-          -exec sh -c 'for f; \
-          do echo $f; \
-          python "$f" || exit 1\
+        run: >-
+          find examples -name "*.py"
+          -exec sh -c 'for f;
+          do echo $f;
+          python "$f" || exit 1
           ; done' sh {} +
```

### Comparing `sleplet-1.3.6/.github/workflows/test.yml` & `sleplet-1.4.0/.github/workflows/test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -18,26 +18,24 @@
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
 
       - name: Cache tox/pooch
         uses: actions/cache@v3
         with:
-          path: |
+          path: |-
             .tox
             ~/.cache/sleplet
           key: test-${{ hashFiles('pyproject.toml') }}
 
       - name: Set up python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install tox tox-gh-actions
+        run: python -m pip install tox tox-gh-actions
 
       - name: Test with tox
         run: tox
```

### Comparing `sleplet-1.3.6/.pre-commit-config.yaml` & `sleplet-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/CONTRIBUTING.md` & `sleplet-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/LICENCE.md` & `sleplet-1.4.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/PKG-INFO` & `sleplet-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.3.6
+Version: 1.4.0
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
         
@@ -69,14 +69,21 @@
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
 
+To read more about Slepian wavelets please see the following publications
+
+[![Sifting Convolution on the Sphere](https://img.shields.io/badge/DOI-10.1109/LSP.2021.3050961-pink.svg)](https://dx.doi.org/10.1109/LSP.2021.3050961)
+[![Slepian Scale-Discretised Wavelets on the Sphere](https://img.shields.io/badge/DOI-10.1109/TSP.2022.3233309-pink.svg)](https://dx.doi.org/10.1109/TSP.2022.3233309)
+[![Slepian Scale-Discretised Wavelets on Manifolds](https://img.shields.io/badge/DOI-10.48550/arXiv.2302.06006-pink.svg)](https://doi.org/10.48550/arXiv.2302.06006)
+[![Slepian Wavelets for the Analysis of Incomplete Data on Manifolds](https://img.shields.io/badge/PhD%20Thesis-Patrick%20J.%20Roddy-pink.svg)](https://paddyroddy.github.io/thesis)
+
 ## Installation
 
 The recommended way to install `SLEPLET` is via
 [pip](https://pypi.org/project/pip)
 
 ```sh
 pip install sleplet
@@ -154,14 +161,26 @@
 ## Community Guidelines
 
 We'd love any contributions you may have, please see the
 [contributing guidelines](https://github.com/astro-informatics/sleplet/blob/main/CONTRIBUTING.md).
 
 ## Citing
 
-If you use `SLEPLET` in your research, please cite the JOSS paper.
-[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
+If you use `SLEPLET` in your research, please cite the paper.
+
+```bibtex
+@article{Roddy2023,
+  title   = {{SLEPLET: Slepian Scale-Discretised Wavelets in Python}},
+  author  = {Roddy, Patrick J.},
+  year    = 2023,
+  journal = {Journal of Open Source Software},
+  volume  = 8,
+  number  = 84,
+  pages   = 5221,
+  doi     = {10.21105/joss.05221},
+}
+```
 
 Please also cite [S2LET](https://doi.org/10.1051/0004-6361/201220729) upon which
 `SLEPLET` is built, along with [SSHT](https://doi.org/10.1109/TSP.2011.2166394)
 in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497)
 in the mesh setting.
```

### Comparing `sleplet-1.3.6/documentation/DOCUMENTATION.md` & `sleplet-1.4.0/documentation/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/documentation/config.mako` & `sleplet-1.4.0/documentation/config.mako`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png` & `sleplet-1.4.0/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png` & `sleplet-1.4.0/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/_denoising_slepian_wavelet.py` & `sleplet-1.4.0/examples/arbitrary/_denoising_slepian_wavelet.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/_slepian_wavelet_covariance.py` & `sleplet-1.4.0/examples/arbitrary/_slepian_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/denoising_slepian_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/denoising_slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/eigenvalues_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/eigenvalues_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/slepian_reconstruction_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/slepian_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/tiling_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/tiling_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/africa/wavelet_reconstruction_africa.py` & `sleplet-1.4.0/examples/arbitrary/africa/wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/eigenvalues_combined.py` & `sleplet-1.4.0/examples/arbitrary/eigenvalues_combined.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/denoising_slepian_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/denoising_slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/eigenvalues_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/eigenvalues_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/slepian_reconstruction_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/slepian_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/tiling_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/tiling_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py` & `sleplet-1.4.0/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/mesh/denoising_slepian_mesh.py` & `sleplet-1.4.0/examples/mesh/denoising_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/mesh/mesh_region.py` & `sleplet-1.4.0/examples/mesh/mesh_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/mesh/mesh_slepian_eigenvalues.py` & `sleplet-1.4.0/examples/mesh/mesh_slepian_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/mesh/mesh_tiling.py` & `sleplet-1.4.0/examples/mesh/mesh_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/misc/_denoising_axisym.py` & `sleplet-1.4.0/examples/misc/_denoising_axisym.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/misc/denoising_axisym_africa.py` & `sleplet-1.4.0/examples/misc/denoising_axisym_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/misc/denoising_axisym_earth.py` & `sleplet-1.4.0/examples/misc/denoising_axisym_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/misc/denoising_axisym_south_america.py` & `sleplet-1.4.0/examples/misc/denoising_axisym_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/misc/translation_normalisation.py` & `sleplet-1.4.0/examples/misc/translation_normalisation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/misc/wavelet_transform.py` & `sleplet-1.4.0/examples/misc/wavelet_transform.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/polar_cap/eigenfunctions.py` & `sleplet-1.4.0/examples/polar_cap/eigenfunctions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/polar_cap/eigenvalues.py` & `sleplet-1.4.0/examples/polar_cap/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/polar_cap/fried_egg.py` & `sleplet-1.4.0/examples/polar_cap/fried_egg.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/polar_cap/simons_5_1.py` & `sleplet-1.4.0/examples/polar_cap/simons_5_1.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/polar_cap/simons_5_3.py` & `sleplet-1.4.0/examples/polar_cap/simons_5_3.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/polar_cap/slepian_coefficients.py` & `sleplet-1.4.0/examples/polar_cap/slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/polar_cap/slepian_error.py` & `sleplet-1.4.0/examples/polar_cap/slepian_error.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/wavelets/axisymmetric_tiling.py` & `sleplet-1.4.0/examples/wavelets/axisymmetric_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/examples/wavelets/axisymmetric_wavelet_covariance.py` & `sleplet-1.4.0/examples/wavelets/axisymmetric_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/paper/paper.bib` & `sleplet-1.4.0/paper/paper.bib`

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 @article{Bates2017,
-  title   = {{Slepian Spatial-Spectral Concentration Problem on the Sphere: Analytical Formulation for Limited Colatitude-Longitude Spatial Region}},
+  title   = {Slepian Spatial-Spectral Concentration Problem on the Sphere: Analytical Formulation for Limited Colatitude-Longitude Spatial Region},
   author  = {Bates, Alice P. and Khalid, Zubair and Kennedy, Rodney A.},
   year    = 2017,
   journal = {IEEE Transactions on Signal Processing},
   volume  = 65,
   number  = 6,
   pages   = {1527--1537},
   doi     = {10.1109/TSP.2016.2646668}
 }
 @article{Harris2020,
-  title   = {{Array programming with NumPy}},
+  title   = {Array programming with {NumPy}},
   author  = {Charles R. Harris and K. Jarrod Millman and St{\'{e}}fan J. van der Walt and Ralf Gommers and Pauli Virtanen and David Cournapeau and Eric Wieser and Julian Taylor and Sebastian Berg and Nathaniel J. Smith and Robert Kern and Matti Picus and Stephan Hoyer and Marten H. van Kerkwijk and Matthew Brett and Allan Haldane and Jaime Fern{\'{a}}ndez del R{\'{i}}o and Mark Wiebe and Pearu Peterson and Pierre G{\'{e}}rard-Marchant and Kevin Sheppard and Tyler Reddy and Warren Weckesser and Hameer Abbasi and Christoph Gohlke and Travis E. Oliphant},
   year    = 2020,
   journal = {Nature},
   volume  = 585,
   number  = 7825,
   pages   = {357--362},
   doi     = {10.1038/s41586-020-2649-2}
 }
 @article{Landau1961,
-  title   = {{Prolate spheroidal wave functions, fourier analysis and uncertainty -- II}},
+  title   = {Prolate spheroidal wave functions, {F}ourier analysis and uncertainty -- {II}},
   author  = {Landau, H. J. and Pollak, H. O.},
   year    = 1961,
   journal = {The Bell System Technical Journal},
   volume  = 40,
   number  = 1,
   pages   = {65--84},
   doi     = {10.1002/j.1538-7305.1961.tb03977.x}
 }
 @article{Landau1962,
-  title   = {{Prolate spheroidal wave functions, fourier analysis and uncertainty -- III: The dimension of the space of essentially time- and band-limited signals}},
+  title   = {Prolate spheroidal wave functions, {F}ourier analysis and uncertainty -- {III}: The dimension of the space of essentially time- and band-limited signals},
   author  = {Landau, H. J. and Pollak, H. O.},
   year    = 1962,
   journal = {The Bell System Technical Journal},
   volume  = 41,
   number  = 4,
   pages   = {1295--1336},
   doi     = {10.1002/j.1538-7305.1962.tb03279.x}
 }
 @article{Leistedt2013,
-  title   = {{S2LET: A code to perform fast wavelet analysis on the sphere}},
+  title   = {S2LET: A code to perform fast wavelet analysis on the sphere},
   author  = {{Leistedt, B.} and {McEwen, J. D.} and {Vandergheynst, P.} and {Wiaux, Y.}},
   year    = 2013,
   journal = {Astronomy \& Astrophysics},
   volume  = 558,
   pages   = {A128},
   doi     = {10.1051/0004-6361/201220729}
 }
 @inproceedings{Libigl2017,
-  title     = {{Libigl: Prototyping Geometry Processing Research in C++}},
+  title     = {Libigl: Prototyping Geometry Processing Research in {C}++},
   author    = {Jacobson, Alec and Panozzo, Daniele},
   year      = 2017,
   booktitle = {SIGGRAPH Asia 2017 Courses},
   publisher = {Association for Computing Machinery},
   doi       = {10.1145/3134472.3134497},
   articleno = 11
 }
 @article{McEwen2011,
-  title   = {{A Novel Sampling Theorem on the Sphere}},
+  title   = {A Novel Sampling Theorem on the Sphere},
   author  = {McEwen, Jason D. and Wiaux, Yves},
   year    = 2011,
   journal = {IEEE Transactions on Signal Processing},
   volume  = 59,
   number  = 12,
   pages   = {5876--5887},
   doi     = {10.1109/TSP.2011.2166394}
 }
 @online{Plotly2015,
-  title  = {{Collaborative data science}},
+  title  = {Collaborative data science},
   author = {Plotly Technologies Inc.},
   year   = 2015,
   url    = {https://plot.ly}
 }
 @article{Roddy2021,
-  title   = {{Sifting Convolution on the Sphere}},
+  title   = {Sifting Convolution on the Sphere},
   author  = {Roddy, Patrick J. and McEwen, Jason D.},
   year    = 2021,
   journal = {IEEE Signal Processing Letters},
   volume  = 28,
   pages   = {304--308},
   doi     = {10.1109/LSP.2021.3050961}
 }
 @article{Roddy2022,
-  title   = {{Slepian Scale-Discretised Wavelets on the Sphere}},
+  title   = {Slepian Scale-Discretised Wavelets on the Sphere},
   author  = {Roddy, Patrick J. and McEwen, Jason D.},
   year    = 2022,
   journal = {IEEE Transactions on Signal Processing},
   volume  = 70,
   pages   = {6142--6153},
   doi     = {10.1109/TSP.2022.3233309}
 }
 @phdthesis{Roddy2022a,
-  title  = {{Slepian Wavelets for the Analysis of Incomplete Data on Manifolds}},
+  title  = {Slepian Wavelets for the Analysis of Incomplete Data on Manifolds},
   author = {Roddy, Patrick J.},
   year   = 2022,
   url    = {https://paddyroddy.github.io/thesis},
   school = {UCL (University College London)}
 }
 @misc{Roddy2023,
-  title     = {{Slepian Scale-Discretised Wavelets on Manifolds}},
+  title     = {Slepian Scale-Discretised Wavelets on Manifolds},
   author    = {Roddy, Patrick J. and McEwen, Jason D.},
   year      = 2023,
   publisher = {arXiv},
   url       = {https://arxiv.org/abs/2302.06006}
 }
 @software{Roddy2023a,
-  title  = {{SLEPLET: Slepian Scale-Discretised Wavelets in Python}},
+  title  = {SLEPLET: {S}lepian Scale-Discretised Wavelets in {P}ython},
   author = {Roddy, Patrick J.},
   year   = 2023,
   doi    = {10.5281/zenodo.7268074}
 }
 @article{Simons2006,
-  title   = {{Spatiospectral Concentration on a Sphere}},
+  title   = {Spatiospectral Concentration on a Sphere},
   author  = {Simons, Frederik J. and Dahlen, F. A. and Wieczorek, Mark A.},
   year    = 2006,
   journal = {SIAM Review},
   volume  = 48,
   number  = 3,
   pages   = {504--536},
   doi     = {10.1137/S0036144504445765}
@@ -123,35 +123,35 @@
 @software{Simons2020,
   title  = {{slepian\_alpha}},
   author = {Frederik J Simons and Chris Harig and Alain Plattner and Max von Hippel and Albert},
   year   = 2020,
   doi    = {10.5281/zenodo.4085210}
 }
 @article{Slepian1961,
-  title   = {{Prolate spheroidal wave functions, fourier analysis and uncertainty -- I}},
+  title   = {Prolate spheroidal wave functions, {F}ourier analysis and uncertainty -- {I}},
   author  = {Slepian, D. and Pollak, H. O.},
   year    = 1961,
   journal = {The Bell System Technical Journal},
   volume  = 40,
   number  = 1,
   pages   = {43--63},
   doi     = {10.1002/j.1538-7305.1961.tb03976.x}
 }
 @article{Wiaux2008,
-  title   = {{Exact reconstruction with directional wavelets on the sphere}},
+  title   = {Exact reconstruction with directional wavelets on the sphere},
   author  = {Wiaux, Y. and McEwen, J. D. and Vandergheynst, P. and Blanc, O.},
   year    = 2008,
   journal = {Monthly Notices of the Royal Astronomical Society},
   volume  = 388,
   number  = 2,
   pages   = {770--788},
   doi     = {10.1111/j.1365-2966.2008.13448.x}
 }
 @article{Wieczorek2018,
-  title   = {{SHTools: Tools for Working with Spherical Harmonics}},
+  title   = {{SHTools}: Tools for Working with Spherical Harmonics},
   author  = {Wieczorek, Mark A. and Meschede, Matthias},
   year    = 2018,
   journal = {Geochemistry, Geophysics, Geosystems},
   volume  = 19,
   number  = 8,
   pages   = {2574--2592},
   doi     = {10.1029/2018GC007529}
```

### Comparing `sleplet-1.3.6/paper/paper.md` & `sleplet-1.4.0/paper/paper.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,48 +16,45 @@
 date: "`r format(Sys.time(), '%d %B %Y')`"
 bibliography: paper.bib
 ---
 
 # Summary
 
 Wavelets are widely used in various disciplines to analyse signals both in space and scale.
-Whilst many fields measure data on manifolds (i.e. the sphere), often data are only observed on a partial region of the manifold.
-Wavelets are a typical approach to data of this form, but the wavelet coefficients which overlap with the boundary become contaminated and must be removed for accurate analysis.
+Whilst many fields measure data on manifolds (i.e., the sphere), often data are only observed on a partial region of the manifold.
+Wavelets are a typical approach to data of this form, but the wavelet coefficients that overlap with the boundary become contaminated and must be removed for accurate analysis.
 Another approach is to estimate the region of missing data and to use existing whole-manifold methods for analysis.
 However, both approaches introduce uncertainty into any analysis.
 Slepian wavelets enable one to work directly with only the data present, thus avoiding the problems discussed above.
-Possible applications of Slepian wavelets to areas of research measuring data on the partial sphere include: gravitational/magnetic fields in geodesy; ground-based measurements in astronomy; measurements of whole-planet properties in planetary science; and geomagnetism of the Earth.
-Slepian wavelets have many potential applications in analyses of manifolds where data are only observed over a partial region.
-One such application is in cosmic microwave background analyses, where observations are inherently made on the celestial sphere, and foreground emissions mask the centre of the data.
-In fields such as astrophysics and cosmology, datasets are increasingly large and thus require analysis at high resolutions for accurate predictions.
+Applications of Slepian wavelets to areas of research measuring data on the partial sphere include gravitational/magnetic fields in geodesy, ground-based measurements in astronomy, measurements of whole-planet properties in planetary science, geomagnetism of the Earth, and cosmic microwave background analyses.
 
 # Statement of Need
 
 Many fields in science and engineering measure data that inherently live on non-Euclidean geometries, such as the sphere.
 Techniques developed in the Euclidean setting must be extended to other geometries.
 Due to recent interest in geometric deep learning, analogues of Euclidean techniques must also handle general manifolds or graphs.
 Often, data are only observed over partial regions of manifolds, and thus standard whole-manifold techniques may not yield accurate predictions.
 Slepian wavelets are designed for datasets like these.
-Slepian wavelets are built upon the eigenfunctions of the Slepian concentration problem of the manifold [@Slepian1961; @Landau1961; @Landau1962] - a set of bandlimited functions which are maximally concentrated within a given region.
+Slepian wavelets are built upon the eigenfunctions of the Slepian concentration problem of the manifold [@Slepian1961; @Landau1961; @Landau1962]: a set of bandlimited functions that are maximally concentrated within a given region.
 Wavelets are constructed through a tiling of the Slepian harmonic line by leveraging the existing scale-discretised framework [@Wiaux2008; @Leistedt2013].
 Whilst these wavelets were inspired by spherical datasets, like in cosmology, the wavelet construction may be utilised for manifold or graph data.
 
-To the author's knowledge, there is no public software which allows one to compute Slepian wavelets
+To the author's knowledge, there is no public software that allows one to compute Slepian wavelets
 (or a similar approach) on the sphere or general manifolds/meshes.
 `SHTools` [@Wieczorek2018] is a `Python` code used for spherical harmonic transforms, which allows one to compute the Slepian functions of the spherical polar cap [@Simons2006].
-A series of `MATLAB` scripts exist in `slepian_alpha` [@Simons2020] which permits the calculation of the Slepian functions on the sphere.
+A series of `MATLAB` scripts exist in `slepian_alpha` [@Simons2020], which permits the calculation of the Slepian functions on the sphere.
 However, these scripts are very specialised and hard to generalise.
 
 `SLEPLET` [@Roddy2023a] is a Python package for the construction of Slepian wavelets in the spherical and manifold (via meshes) settings.
 In contrast to the aforementioned codes, `SLEPLET` handles any spherical region as well as the general manifold setting.
 The API is documented and easily extendible, designed in an object-orientated manner.
-Upon installation, `SLEPLET` comes with two command line interfaces - `sphere` and `mesh` - which allows one to easily generate plots on the sphere and a set of meshes using `plotly`.
+Upon installation, `SLEPLET` comes with two command line interfaces - `sphere` and `mesh` - that allow one to easily generate plots on the sphere and a set of meshes using `plotly`.
 Whilst these scripts are the primary intended use, `SLEPLET` may be used directly to generate the Slepian coefficients in the spherical/manifold setting and use methods to convert these into real space for visualisation or other intended purposes.
 The construction of the sifting convolution [@Roddy2021] was required to create Slepian wavelets.
-As a result, there are also many examples of functions on the sphere in harmonic space (rather than Slepian) which were used to demonstrate its effectiveness.
+As a result, there are also many examples of functions on the sphere in harmonic space (rather than Slepian) that were used to demonstrate its effectiveness.
 `SLEPLET` has been used in the development of [@Roddy2021; @Roddy2022; @Roddy2022a; @Roddy2023].
 
 Whilst Slepian wavelets may be trivially computed from a set of Slepian functions, the computation of the spherical Slepian functions themselves are computationally complex, where the matrix scales as $\mathcal{O}(L^{4})$.
 Although symmetries of this matrix and the spherical harmonics have been exploited, filling in this matrix is inherently slow due to the many integrals performed.
 The matrix is filled in parallel in `Python` using `concurrent.futures`, and the spherical harmonic transforms are computed in `C` using `SSHT`.
 This may be sped up further by utilising the new `ducc0` backend for `SSHT`, which may allow for a multithreaded solution.
 Ultimately, the eigenproblem must be solved to compute the Slepian functions, requiring sophisticated algorithms to balance speed and accuracy.
```

### Comparing `sleplet-1.3.6/pyproject.toml` & `sleplet-1.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -49,38 +49,32 @@
     "manifolds",
     "python",
     "slepian-functions",
     "sphere",
     "wavelets",
 ]
 name = "sleplet"
-readme = "README.md"
-requires-python = ">=3.10"
-scripts = {mesh = "sleplet._scripts.plotting_on_mesh:main", sphere = "sleplet._scripts.plotting_on_sphere:main"}
-license.file = "LICENCE.md"
-optional-dependencies.dev = [
+optional-dependencies = {dev = [
     "black",
     "build",
     "mypy",
     "pre-commit",
     "ruff",
     "tox",
     "twine",
-]
-optional-dependencies.docs = [
+], docs = [
     "pdoc3",
-]
-optional-dependencies.readme = [
+], readme = [
     "pytest-codeblocks",
-]
-urls.Code = "https://github.com/astro-informatics/sleplet"
-urls.Documentation = "https://astro-informatics.github.io/sleplet"
-urls.Download = "https://pypi.org/project/sleplet"
-urls.Homepage = "https://github.com/astro-informatics/sleplet"
-urls.Issues = "https://github.com/astro-informatics/sleplet/issues"
+]}
+readme = "README.md"
+requires-python = ">=3.10"
+scripts = {mesh = "sleplet._scripts.plotting_on_mesh:main", sphere = "sleplet._scripts.plotting_on_sphere:main"}
+urls = {Code = "https://github.com/astro-informatics/sleplet", Documentation = "https://astro-informatics.github.io/sleplet", Download = "https://pypi.org/project/sleplet", Homepage = "https://github.com/astro-informatics/sleplet", Issues = "https://github.com/astro-informatics/sleplet/issues"}
+license.file = "LICENCE.md"
 
 [tool.coverage]
 report = {skip_covered = true, sort = "cover"}
 run = {branch = true, parallel = true, source = ["sleplet"]}
 paths.source = [
     "src",
     ".tox*/*/lib/python*/site-packages",
```

### Comparing `sleplet-1.3.6/src/sleplet/__init__.py` & `sleplet-1.4.0/src/sleplet/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_bool_methods.py` & `sleplet-1.4.0/src/sleplet/_bool_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_class_lists.py` & `sleplet-1.4.0/src/sleplet/_class_lists.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_convolution_methods.py` & `sleplet-1.4.0/src/sleplet/_convolution_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/create_earth_flm.py` & `sleplet-1.4.0/src/sleplet/_data/create_earth_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/create_wmap_flm.py` & `sleplet-1.4.0/src/sleplet/_data/create_wmap_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_bird.off` & `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_bird.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cheetah.off` & `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cheetah.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_cube.off` & `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_cube.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_dragon.off` & `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_dragon.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_homer.off` & `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_homer.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/meshes_polygons_teapot.off` & `sleplet-1.4.0/src/sleplet/_data/meshes_polygons_teapot.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_data/setup_pooch.py` & `sleplet-1.4.0/src/sleplet/_data/setup_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_integration_methods.py` & `sleplet-1.4.0/src/sleplet/_integration_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_mask_methods.py` & `sleplet-1.4.0/src/sleplet/_mask_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_mesh_methods.py` & `sleplet-1.4.0/src/sleplet/_mesh_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_parallel_methods.py` & `sleplet-1.4.0/src/sleplet/_parallel_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_plotly_methods.py` & `sleplet-1.4.0/src/sleplet/_plotly_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_scripts/plotting_on_mesh.py` & `sleplet-1.4.0/src/sleplet/_scripts/plotting_on_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_scripts/plotting_on_sphere.py` & `sleplet-1.4.0/src/sleplet/_scripts/plotting_on_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_slepian_arbitrary_methods.py` & `sleplet-1.4.0/src/sleplet/_slepian_arbitrary_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_smoothing.py` & `sleplet-1.4.0/src/sleplet/_smoothing.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/_string_methods.py` & `sleplet-1.4.0/src/sleplet/_string_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/__init__.py` & `sleplet-1.4.0/src/sleplet/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/africa.py` & `sleplet-1.4.0/src/sleplet/functions/africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py` & `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py` & `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py` & `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/axisymmetric_wavelets.py` & `sleplet-1.4.0/src/sleplet/functions/axisymmetric_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/coefficients.py` & `sleplet-1.4.0/src/sleplet/functions/coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/dirac_delta.py` & `sleplet-1.4.0/src/sleplet/functions/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/directional_spin_wavelets.py` & `sleplet-1.4.0/src/sleplet/functions/directional_spin_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/earth.py` & `sleplet-1.4.0/src/sleplet/functions/earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/elongated_gaussian.py` & `sleplet-1.4.0/src/sleplet/functions/elongated_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/flm.py` & `sleplet-1.4.0/src/sleplet/functions/flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/fp.py` & `sleplet-1.4.0/src/sleplet/functions/fp.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/gaussian.py` & `sleplet-1.4.0/src/sleplet/functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/harmonic_gaussian.py` & `sleplet-1.4.0/src/sleplet/functions/harmonic_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/identity.py` & `sleplet-1.4.0/src/sleplet/functions/identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/noise_earth.py` & `sleplet-1.4.0/src/sleplet/functions/noise_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/ridgelets.py` & `sleplet-1.4.0/src/sleplet/functions/ridgelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian.py` & `sleplet-1.4.0/src/sleplet/functions/slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_africa.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_dirac_delta.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_identity.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_noise_africa.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_noise_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_noise_south_america.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_noise_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_south_america.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_africa.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/slepian_wavelets.py` & `sleplet-1.4.0/src/sleplet/functions/slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/south_america.py` & `sleplet-1.4.0/src/sleplet/functions/south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/spherical_harmonic.py` & `sleplet-1.4.0/src/sleplet/functions/spherical_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/squashed_gaussian.py` & `sleplet-1.4.0/src/sleplet/functions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/functions/wmap.py` & `sleplet-1.4.0/src/sleplet/functions/wmap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/harmonic_methods.py` & `sleplet-1.4.0/src/sleplet/harmonic_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/__init__.py` & `sleplet-1.4.0/src/sleplet/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/_mesh_slepian_decomposition.py` & `sleplet-1.4.0/src/sleplet/meshes/_mesh_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_basis_functions.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_basis_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_coefficients.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_field.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_harmonic_coefficients.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_harmonic_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_noise_field.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_coefficients.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_field.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_functions.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_noise_field.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/meshes/mesh_slepian_wavelets.py` & `sleplet-1.4.0/src/sleplet/meshes/mesh_slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/noise.py` & `sleplet-1.4.0/src/sleplet/noise.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/plot_methods.py` & `sleplet-1.4.0/src/sleplet/plot_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/plotting/_create_plot_mesh.py` & `sleplet-1.4.0/src/sleplet/plotting/_create_plot_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/plotting/_create_plot_sphere.py` & `sleplet-1.4.0/src/sleplet/plotting/_create_plot_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/slepian/_slepian_decomposition.py` & `sleplet-1.4.0/src/sleplet/slepian/_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/slepian/region.py` & `sleplet-1.4.0/src/sleplet/slepian/region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/slepian/slepian_arbitrary.py` & `sleplet-1.4.0/src/sleplet/slepian/slepian_arbitrary.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/slepian/slepian_functions.py` & `sleplet-1.4.0/src/sleplet/slepian/slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/slepian/slepian_limit_lat_lon.py` & `sleplet-1.4.0/src/sleplet/slepian/slepian_limit_lat_lon.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/slepian/slepian_polar_cap.py` & `sleplet-1.4.0/src/sleplet/slepian/slepian_polar_cap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/slepian_methods.py` & `sleplet-1.4.0/src/sleplet/slepian_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet/wavelet_methods.py` & `sleplet-1.4.0/src/sleplet/wavelet_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/src/sleplet.egg-info/PKG-INFO` & `sleplet-1.4.0/src/sleplet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.3.6
+Version: 1.4.0
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
         
@@ -69,14 +69,21 @@
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
 
+To read more about Slepian wavelets please see the following publications
+
+[![Sifting Convolution on the Sphere](https://img.shields.io/badge/DOI-10.1109/LSP.2021.3050961-pink.svg)](https://dx.doi.org/10.1109/LSP.2021.3050961)
+[![Slepian Scale-Discretised Wavelets on the Sphere](https://img.shields.io/badge/DOI-10.1109/TSP.2022.3233309-pink.svg)](https://dx.doi.org/10.1109/TSP.2022.3233309)
+[![Slepian Scale-Discretised Wavelets on Manifolds](https://img.shields.io/badge/DOI-10.48550/arXiv.2302.06006-pink.svg)](https://doi.org/10.48550/arXiv.2302.06006)
+[![Slepian Wavelets for the Analysis of Incomplete Data on Manifolds](https://img.shields.io/badge/PhD%20Thesis-Patrick%20J.%20Roddy-pink.svg)](https://paddyroddy.github.io/thesis)
+
 ## Installation
 
 The recommended way to install `SLEPLET` is via
 [pip](https://pypi.org/project/pip)
 
 ```sh
 pip install sleplet
@@ -154,14 +161,26 @@
 ## Community Guidelines
 
 We'd love any contributions you may have, please see the
 [contributing guidelines](https://github.com/astro-informatics/sleplet/blob/main/CONTRIBUTING.md).
 
 ## Citing
 
-If you use `SLEPLET` in your research, please cite the JOSS paper.
-[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
+If you use `SLEPLET` in your research, please cite the paper.
+
+```bibtex
+@article{Roddy2023,
+  title   = {{SLEPLET: Slepian Scale-Discretised Wavelets in Python}},
+  author  = {Roddy, Patrick J.},
+  year    = 2023,
+  journal = {Journal of Open Source Software},
+  volume  = 8,
+  number  = 84,
+  pages   = 5221,
+  doi     = {10.21105/joss.05221},
+}
+```
 
 Please also cite [S2LET](https://doi.org/10.1051/0004-6361/201220729) upon which
 `SLEPLET` is built, along with [SSHT](https://doi.org/10.1109/TSP.2011.2166394)
 in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497)
 in the mesh setting.
```

### Comparing `sleplet-1.3.6/src/sleplet.egg-info/SOURCES.txt` & `sleplet-1.4.0/src/sleplet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 examples/polar_cap/fried_egg.py
 examples/polar_cap/simons_5_1.py
 examples/polar_cap/simons_5_3.py
 examples/polar_cap/slepian_coefficients.py
 examples/polar_cap/slepian_error.py
 examples/wavelets/axisymmetric_tiling.py
 examples/wavelets/axisymmetric_wavelet_covariance.py
+paper/arxiv.tex
 paper/paper.bib
 paper/paper.md
 src/sleplet/__init__.py
 src/sleplet/_array_methods.py
 src/sleplet/_bool_methods.py
 src/sleplet/_class_lists.py
 src/sleplet/_convolution_methods.py
```

### Comparing `sleplet-1.3.6/tests/conftest.py` & `sleplet-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_arbitrary_region.py` & `sleplet-1.4.0/tests/test_arbitrary_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_arrays.py` & `sleplet-1.4.0/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_bool.py` & `sleplet-1.4.0/tests/test_bool.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_convolution.py` & `sleplet-1.4.0/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_decomposition.py` & `sleplet-1.4.0/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_harmonic.py` & `sleplet-1.4.0/tests/test_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_loading_pooch.py` & `sleplet-1.4.0/tests/test_loading_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_mesh.py` & `sleplet-1.4.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_plot.py` & `sleplet-1.4.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_region.py` & `sleplet-1.4.0/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_slepian_mesh.py` & `sleplet-1.4.0/tests/test_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_strings.py` & `sleplet-1.4.0/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_translation.py` & `sleplet-1.4.0/tests/test_translation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.3.6/tests/test_wavelets.py` & `sleplet-1.4.0/tests/test_wavelets.py`

 * *Files identical despite different names*

