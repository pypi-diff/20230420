# Comparing `tmp/chia-blockchain-1.8.0b6.tar.gz` & `tmp/chia-blockchain-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chia-blockchain-1.8.0b6.tar", last modified: Mon Apr 17 22:35:09 2023, max compression
+gzip compressed data, was "chia-blockchain-1.8.0rc1.tar", last modified: Thu Apr 20 03:20:39 2023, max compression
```

## Comparing `chia-blockchain-1.8.0b6.tar` & `chia-blockchain-1.8.0rc1.tar`

### file list

```diff
@@ -1,1105 +1,1066 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.356978 chia-blockchain-1.8.0b6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.356978 chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.344978 chia-blockchain-1.8.0b6/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.356978 chia-blockchain-1.8.0b6/.github/actions/install/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/actions/install/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-linux-arm64-installer.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-deb.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-macos-installers.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-windows-installer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/check-commit-signing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/check_wheel_availability.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/conflict-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/mozilla-ca-cert.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/require-labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/snyk-python-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/start-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/start-sync-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/super-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/test-install-scripts.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/test-single.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/upload-pypi-source.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.markdown-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/BUILD_TIMELORD.md
--rw-r--r--   0 runner    (1001) docker     (123)   207286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/Install-gui.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/Install-plotter.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/Install.ps1
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33099 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/PRETTY_GOOD_PRACTICES.md
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/activated.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/activated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/activated.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/block_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   121543 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/clvm_generator.bin
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/jsonify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/mempool-long-lived.py
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/mempool.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)   439288 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/transaction_height_delta
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/build_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/build_scripts/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/build_scripts/assets/deb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/control.j2
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/postinst.sh
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/prerm.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/README
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   507222 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/background.tiff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/postinst.sh
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/prerm.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-1-gui.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-2-installer.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-1-gui.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-2-installer.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_macos-1-gui.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_macos-2-installer.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_windows-1-gui.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_windows-2-installer.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/check_dependency_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/clean-runner.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/installer-version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_global/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_global/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_global/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_global/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   539731 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_linux/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_linux/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   572329 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_macos/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_macos/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   553007 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_windows/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_windows/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.368978 chia-blockchain-1.8.0b6/chia/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.368978 chia-blockchain-1.8.0b6/chia/clvm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/clvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/clvm/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/clvm/spend_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.372978 chia-blockchain-1.8.0b6/chia/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/beta_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/check_wallet_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/chia.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/cmds_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/coin_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/coins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db_backup_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    17725 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db_upgrade_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db_validate_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/farm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/farm_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/init_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/keys_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/netspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/netspace_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/passphrase_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/peer_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plotnft.py
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plotnft_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/show_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/start_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    38959 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)    49571 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/wallet_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_body_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    51022 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_header_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_root_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    42752 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/blockchain_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/condition_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/cost_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/default_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/difficulty_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/find_fork_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/full_block_to_block_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/get_block_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/make_sub_epoch_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18835 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/multiprocess_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/pos_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/pot_iterations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/vdf_info_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/keychain_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/keychain_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    56085 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/windows_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/data_layer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38872 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    62659 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)    62999 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/dl_wallet_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/download_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/s3_plugin_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/s3_plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/data_layer/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/util/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/farmer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/farmer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36468 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/farmer/farmer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28233 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/farmer/farmer_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.380978 chia-blockchain-1.8.0b6/chia/full_node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/bitcoin_fee_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/block_height_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    32512 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/bundle_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    22559 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)   130083 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/full_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    79298 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/full_node_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36689 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/full_node_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/hint_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/hint_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/lock_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/mempool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/mempool_check_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33485 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/mempool_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/pending_tx_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/signage_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/sync_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/tx_processing_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    72530 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/weight_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.380978 chia-blockchain-1.8.0b6/chia/harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/harvester/harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/harvester/harvester_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.380978 chia-blockchain-1.8.0b6/chia/introducer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/introducer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/introducer/introducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/introducer/introducer_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/plot_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/bladebit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/chiapos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/madmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/plotters_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/check_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/create_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/pools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)    44516 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_wallet_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/farmer_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/full_node_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/harvester_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/introducer_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/pool_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/protocol_message_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/protocol_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/protocol_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/shared_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/timelord_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/wallet_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pyinstaller.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.388978 chia-blockchain-1.8.0b6/chia/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/crawler_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/timelord_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/util.py
--rw-r--r--   0 runner    (1001) docker     (123)   160950 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    44813 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.388978 chia-blockchain-1.8.0b6/chia/seeder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/crawl_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/crawler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/dns_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/peer_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/start_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.392978 chia-blockchain-1.8.0b6/chia/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27079 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/address_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/address_manager_sqlite_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/address_manager_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/chia_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/introducer_peers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33202 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/node_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/outbound_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/peer_store_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/rate_limit_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/rate_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/ssl_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_data_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_farmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_full_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_introducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_timelord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/upnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/ws_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.396978 chia-blockchain-1.8.0b6/chia/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95653 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/block_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    28844 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/full_node_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/setup_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/setup_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    39473 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_10.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39471 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_3.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_4.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_5.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_6.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_7.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_8.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/start_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/time_out_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/wallet_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.396978 chia-blockchain-1.8.0b6/chia/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/chia_ca.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/chia_ca.key
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/create_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/dst_root_ca.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.396978 chia-blockchain-1.8.0b6/chia/timelord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/iters_from_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    58402 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.400978 chia-blockchain-1.8.0b6/chia/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/block_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.400978 chia-blockchain-1.8.0b6/chia/types/blockchain_format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/classgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/foliage.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/pool_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/proof_of_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/reward_chain_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/serialized_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/sized_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/sub_epoch_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/tree_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/vdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/clvm_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/coin_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/coin_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/coin_spend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/condition_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/condition_with_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/end_of_slot_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/fee_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/full_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/generator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/header_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mempool_inclusion_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mempool_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mempool_submission_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mojos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/peer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/signing_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/spend_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/spend_bundle_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/transaction_queue_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/unfinished_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/unfinished_header_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/weight_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.408978 chia-blockchain-1.8.0b6/chia/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/api_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/bech32m.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/beta_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/block_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/byte_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/cached_bls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/check_fork_next_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/chia_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/condition_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/create_alert_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/db_synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/db_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/db_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/default_root.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2866 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/dump_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/english.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/file_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/full_block_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/generator_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    24198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/initial-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/inline_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/ints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/keyring_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/limited_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/log_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/make_test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/merkle_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/partial_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/prev_transaction_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/recursive_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/safe_cancel_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/setproctitle.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/significant_bits.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/ssl_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/struct_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/task_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/validate_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/vdf_prover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/ws_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/block_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42955 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/lineage_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/chialisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/coin_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/dao_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/dao_wallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/db_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/db_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/db_wallet/db_wallet_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/derivation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/derive_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.416978 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    62287 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/driver_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/key_val_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/lineage_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.416978 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/metadata_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)    83964 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/ownership_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/singleton_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/transfer_program_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/uncurry_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/notification_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/notification_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/outer_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzle_drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.432978 chia-blockchain-1.8.0b6/chia/wallet/puzzles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/calculate_synthetic_public_key.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_truths.clib
--rw-r--r--   0 runner    (1001) docker     (123)    17221 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/condition_codes.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create-lock-puzzlehash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create_nft_launcher_from_did.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry-and-treehash.clinc
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry.clib
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/everything_with_signature.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/everything_with_signature.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/everything_with_signature.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/json.clib
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/load_clvm.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/lock.inner.puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/lock.inner.puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/lock.inner.puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/merkle_utils.clib
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_intermediate_launcher.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/notification.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/notification.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/notification.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_parent.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_parent.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_parent.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex.sha256tree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.432978 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/make_prefarm_ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/spend_prefarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/puzzle_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/recompile-all.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree.clib
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree_module.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree_module.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree_module.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_launcher.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_launcher.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_launcher.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_truths.clib
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/tails.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_generator_deserialize.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_generator_deserialize.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_generator_deserialize.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/utility_macros.clib
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/secret_key_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/sign_coin_spends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    43570 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trade_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trade_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.432978 chia-blockchain-1.8.0b6/chia/wallet/trading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32738 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/trade_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/trade_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/transaction_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/transaction_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/uncurried_puzzle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/chia/wallet/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/address_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/compute_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/compute_memos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/curry_and_treehash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/debug_spend_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/json_clvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/merkle_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/merkle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/new_peak_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/peer_request_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/puzzle_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/wallet_sync_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/wallet_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    27732 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_coin_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_interested_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_nft_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    80370 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_node_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_pool_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_puzzle_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_retry_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    86139 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_transaction_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_user_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_weight_proof_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:30:52.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     6676 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install-gui.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4910 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install-plotter.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install-timelord.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    12552 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/installhelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/mozilla-ca/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:31.000000 chia-blockchain-1.8.0b6/mozilla-ca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   216583 2023-04-17 22:30:31.000000 chia-blockchain-1.8.0b6/mozilla-ca/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/run-py-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/start-gui.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.440977 chia-blockchain-1.8.0b6/tests/blockchain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/blockchain_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   166834 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    37614 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2431 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/build-init-files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/build-job-matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/check_pytest_monitor_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2398 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/check_sql_statements.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1750 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/chia-start-sim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.440977 chia-blockchain-1.8.0b6/tests/clvm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/benchmark_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_chialisp_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_clvm_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_curry_and_treehash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_serialized_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_spend_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.440977 chia-blockchain-1.8.0b6/tests/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/cmds/test_wallet_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    28614 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/connection_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/test_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)    38994 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/test_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/consensus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/consensus/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/consensus/test_pot_iterations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/custom_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/test_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/test_proof_of_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/test_spend_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/test_keychain_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/data_layer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_layer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)   245364 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47306 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/dos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/dos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/dos/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/test_full_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/ram_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    34130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_full_node_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_hint_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_sync_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_address_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_block_height_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    87563 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_full_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_generator_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_hint_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_node_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_peer_store_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_tx_processing_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)   187863 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/large_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/make_block_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/mempool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   123916 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/node_height.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/core/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/flood.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_dos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_rate_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_upnp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/core/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/ssl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/ssl/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_coins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_cost_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_crawler_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_daemon_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_db_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_db_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23550 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_farmer_harvester_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_full_node_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_merkle_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_setproctitle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_cached_bls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_file_keyring_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_jsonify.py
--rw-r--r--   0 runner    (1001) docker     (123)    20681 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)    22952 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_keyring_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_significant_bits.py
--rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_streamable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/db/test_db_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/farmer_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/farmer_harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/farmer_harvester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/farmer_harvester/test_farmer_harvester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/fee_estimation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/cmdline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_unit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_mempoolitem_height_added.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_generator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_list_to_batches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_rom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/plot_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    29365 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_plot_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_sync_simulated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32802 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/test_plot_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/pools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_puzzles_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    47263 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_wallet_pool_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/test_start_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/testconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.460977 chia-blockchain-1.8.0b6/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/1315537.json
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/1315544.json
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/1315630.json
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/300000.json
--rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/442734.json
--rw-r--r--   0 runner    (1001) docker     (123)   233251 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/466212.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   405504 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test-blockchain-db.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test_full_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test_legacy_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test_run_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.464977 chia-blockchain-1.8.0b6/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/alert_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/benchmark_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/bip39_test_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/build_network_protocol_files.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/gen_ssl_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/generator_tools_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/key_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/network_protocol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/protocol_messages_bytes-v1.0
--rw-r--r--   0 runner    (1001) docker     (123)   170660 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/protocol_messages_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/temp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_full_block_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_limited_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_lock_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    22379 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network_protocol_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network_protocol_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network_protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_struct_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_trusted_peer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25164 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39540 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_offer_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)   162923 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_trades.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/dao_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/dao_wallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_db_graftroot.py
--rw-r--r--   0 runner    (1001) docker     (123)   135852 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    65884 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/test_did.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   374078 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_1_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)    43345 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_bulk_mint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    66774 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)    76327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/wallet/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/test_dl_wallet_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    74646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/test_wallet_rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/test_simple_sync_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/wallet/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    65523 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/sync/test_wallet_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_address_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_bech32m.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_chialisp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_coin_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_nft_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_offer_parsing_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_puzzle_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_taproot.py
--rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_transaction_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    43806 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_interested_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_key_val_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_trade_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_user_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/weight_proof/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/weight_proof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/weight_proof/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/weight_proof/test_weight_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/analyze-chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/analyze_memory_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/cpu_utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/generate_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/legacy_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/manage_clvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/plot-log.gnuplot
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/run_benchmark.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/run_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/test_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13441 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/test_full_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.447016 chia-blockchain-1.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.323016 chia-blockchain-1.8.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.323016 chia-blockchain-1.8.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.311016 chia-blockchain-1.8.0rc1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.323016 chia-blockchain-1.8.0rc1/.github/actions/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/actions/install/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.327016 chia-blockchain-1.8.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/build-linux-arm64-installer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/build-linux-installer-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/build-linux-installer-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/build-macos-installers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/build-windows-installer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/check-commit-signing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/check_wheel_availability.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/conflict-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/daily-matrix.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/mozilla-ca-cert.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/require-labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/snyk-python-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/start-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/start-sync-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/super-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/test-install-scripts.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/test-single.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/trigger-docker-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/trigger-docker-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.github/workflows/upload-pypi-source.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.markdown-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/BUILD_TIMELORD.md
+-rw-r--r--   0 runner    (1001) docker     (123)   207286 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/Install-gui.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/Install-plotter.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/Install.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-20 03:20:39.447016 chia-blockchain-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33099 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/PRETTY_GOOD_PRACTICES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/activated.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/activated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      155 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/activated.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.327016 chia-blockchain-1.8.0rc1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/block_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121543 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/clvm_generator.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/jsonify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/mempool-long-lived.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/mempool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)   439288 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/transaction_height_delta
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.331016 chia-blockchain-1.8.0rc1/build_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.331016 chia-blockchain-1.8.0rc1/build_scripts/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.331016 chia-blockchain-1.8.0rc1/build_scripts/assets/deb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/deb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/deb/control.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/deb/postinst.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/deb/prerm.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.331016 chia-blockchain-1.8.0rc1/build_scripts/assets/dmg/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/dmg/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/dmg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   507222 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/dmg/background.tiff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.331016 chia-blockchain-1.8.0rc1/build_scripts/assets/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/rpm/postinst.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/assets/rpm/prerm.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_linux_deb-1-gui.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_linux_deb-2-installer.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_linux_rpm-1-gui.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_linux_rpm-2-installer.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_macos-1-gui.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_macos-2-installer.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_windows-1-gui.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/build_windows-2-installer.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/check_dependency_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/clean-runner.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/installer-version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.331016 chia-blockchain-1.8.0rc1/build_scripts/npm_global/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_global/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_global/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_global/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.335016 chia-blockchain-1.8.0rc1/build_scripts/npm_linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539731 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_linux/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_linux/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.335016 chia-blockchain-1.8.0rc1/build_scripts/npm_macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   572329 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_macos/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_macos/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.335016 chia-blockchain-1.8.0rc1/build_scripts/npm_windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   553007 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_windows/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/build_scripts/npm_windows/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.335016 chia-blockchain-1.8.0rc1/chia/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.335016 chia-blockchain-1.8.0rc1/chia/clvm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/clvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/clvm/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/clvm/spend_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.343016 chia-blockchain-1.8.0rc1/chia/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/beta_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/check_wallet_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/chia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/cmds_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/coin_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/coins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/db_backup_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17725 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/db_upgrade_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/db_validate_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/farm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/farm_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/init_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/keys_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/netspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/netspace_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/passphrase_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/peer_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/plotnft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/plotnft_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/show_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/sim_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/start_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38959 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49653 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/cmds/wallet_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.347016 chia-blockchain-1.8.0rc1/chia/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/block_body_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/block_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51022 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/block_header_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/block_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/block_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/block_root_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42752 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/blockchain_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/condition_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/cost_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/default_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/difficulty_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/find_fork_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/full_block_to_block_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/get_block_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/make_sub_epoch_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18835 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/multiprocess_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/pos_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/pot_iterations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/consensus/vdf_info_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.347016 chia-blockchain-1.8.0rc1/chia/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/daemon/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/daemon/keychain_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/daemon/keychain_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56085 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/daemon/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/daemon/windows_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.347016 chia-blockchain-1.8.0rc1/chia/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/data_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62475 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62999 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/dl_wallet_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/s3_plugin_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/s3_plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.347016 chia-blockchain-1.8.0rc1/chia/data_layer/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/data_layer/util/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.347016 chia-blockchain-1.8.0rc1/chia/farmer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/farmer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36468 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/farmer/farmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28233 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/farmer/farmer_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.355016 chia-blockchain-1.8.0rc1/chia/full_node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/bitcoin_fee_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/block_height_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32512 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/bundle_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_estimate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22559 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/fee_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130083 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/full_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79298 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/full_node_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36689 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/full_node_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/hint_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/hint_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/lock_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/mempool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/mempool_check_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33485 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/mempool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/pending_tx_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/signage_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/sync_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/tx_processing_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72530 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/full_node/weight_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.355016 chia-blockchain-1.8.0rc1/chia/harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/harvester/harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/harvester/harvester_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.355016 chia-blockchain-1.8.0rc1/chia/introducer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/introducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/introducer/introducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/introducer/introducer_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.355016 chia-blockchain-1.8.0rc1/chia/plot_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plot_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plot_sync/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plot_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plot_sync/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plot_sync/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plot_sync/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.355016 chia-blockchain-1.8.0rc1/chia/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotters/bladebit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotters/chiapos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotters/madmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotters/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotters/plotters_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.355016 chia-blockchain-1.8.0rc1/chia/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotting/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotting/check_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotting/create_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotting/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/plotting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.355016 chia-blockchain-1.8.0rc1/chia/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/pools/pool_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/pools/pool_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44516 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/pools/pool_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/pools/pool_wallet_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.359016 chia-blockchain-1.8.0rc1/chia/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/farmer_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/full_node_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/harvester_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/introducer_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/pool_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/protocol_message_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/protocol_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/protocol_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/shared_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/timelord_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/protocols/wallet_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/pyinstaller.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.359016 chia-blockchain-1.8.0rc1/chia/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/crawler_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/data_layer_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/data_layer_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/data_layer_rpc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/farmer_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/farmer_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41327 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/full_node_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/full_node_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/harvester_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/harvester_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/timelord_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160800 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/wallet_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44813 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/rpc/wallet_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.363016 chia-blockchain-1.8.0rc1/chia/seeder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/seeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/seeder/crawl_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/seeder/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/seeder/crawler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/seeder/dns_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/seeder/peer_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/seeder/start_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.367016 chia-blockchain-1.8.0rc1/chia/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27079 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/address_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/address_manager_sqlite_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/address_manager_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/chia_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/introducer_peers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33084 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/node_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/outbound_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/peer_store_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/rate_limit_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/rate_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/ssl_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_data_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_farmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_full_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_introducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_timelord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/start_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/upnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/server/ws_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.371016 chia-blockchain-1.8.0rc1/chia/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96083 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/block_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28844 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/full_node_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/setup_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/setup_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/simulator_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/simulator_full_node_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/simulator_full_node_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/simulator_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/simulator_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39473 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39471 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/start_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/time_out_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/simulator/wallet_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.371016 chia-blockchain-1.8.0rc1/chia/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/ssl/chia_ca.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/ssl/chia_ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/ssl/create_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/ssl/dst_root_ca.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.371016 chia-blockchain-1.8.0rc1/chia/timelord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/timelord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/timelord/iters_from_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58402 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/timelord/timelord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/timelord/timelord_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/timelord/timelord_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/timelord/timelord_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/timelord/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.375016 chia-blockchain-1.8.0rc1/chia/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/block_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.375016 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/classgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/foliage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/pool_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/proof_of_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/reward_chain_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/serialized_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/sized_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/sub_epoch_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/tree_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/blockchain_format/vdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/clvm_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/coin_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/coin_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/coin_spend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/condition_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/condition_with_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/end_of_slot_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/fee_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/full_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/generator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/header_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/mempool_inclusion_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/mempool_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/mempool_submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/mojos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/peer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/signing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/spend_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/spend_bundle_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/transaction_queue_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/unfinished_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/unfinished_header_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/types/weight_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.383016 chia-blockchain-1.8.0rc1/chia/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/api_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/bech32m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/beta_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/block_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/byte_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/cached_bls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/check_fork_next_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/chia_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/condition_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/create_alert_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/db_synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/db_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/db_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/default_root.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2866 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/dump_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/english.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/file_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/full_block_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/generator_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24263 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/initial-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/inline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/ints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/keyring_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/limited_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/log_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/make_test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/merkle_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/partial_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/prev_transaction_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/recursive_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/safe_cancel_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/setproctitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/significant_bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/ssl_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/struct_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/task_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/validate_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/vdf_prover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/util/ws_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.391016 chia-blockchain-1.8.0rc1/chia/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/block_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.391016 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42935 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/lineage_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/chialisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/coin_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.391016 chia-blockchain-1.8.0rc1/chia/wallet/dao_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/dao_wallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.391016 chia-blockchain-1.8.0rc1/chia/wallet/db_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/db_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/db_wallet/db_wallet_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/derivation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/derive_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.391016 chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/did_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62342 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/did_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/did_wallet_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/driver_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/key_val_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/lineage_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.391016 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/metadata_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/nft_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/nft_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84011 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/nft_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/ownership_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/singleton_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/transfer_program_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/uncurry_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/notification_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/notification_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/outer_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzle_drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.403016 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/block_program_zero.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/block_program_zero.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/calculate_synthetic_public_key.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/calculate_synthetic_public_key.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/cat_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/cat_truths.clib
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/cat_v2.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/cat_v2.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/chialisp_deserialisation.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/chialisp_deserialisation.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/condition_codes.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/create-lock-puzzlehash.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/create_nft_launcher_from_did.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/create_nft_launcher_from_did.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/curry-and-treehash.clib
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/curry.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/decompress_coin_spend_entry.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/decompress_coin_spend_entry.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/decompress_puzzle.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/decompress_puzzle.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/delegated_tail.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/delegated_tail.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/deployed_puzzle_hashes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/did_innerpuz.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/did_innerpuz.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/everything_with_signature.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/everything_with_signature.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/genesis_by_coin_id.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/genesis_by_coin_id.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/genesis_by_puzzle_hash.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/genesis_by_puzzle_hash.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/graftroot_dl_offers.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/graftroot_dl_offers.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/json.clib
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/load_clvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/merkle_utils.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_intermediate_launcher.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_intermediate_launcher.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_metadata_updater_default.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_metadata_updater_default.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_metadata_updater_updateable.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_metadata_updater_updateable.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_layer.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_layer.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_state_layer.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_state_layer.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/notification.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/notification.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_conditions.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_conditions.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_conditions.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_conditions.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_parent.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_parent.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_puzzle_hash.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_puzzle_hash.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_puzzle_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_member_innerpuz.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_member_innerpuz.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_waitingroom_innerpuz.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_waitingroom_innerpuz.clsp.hex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.403016 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/prefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/prefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/prefarm/make_prefarm_ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/prefarm/spend_prefarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/puzzle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/rom_bootstrap_generator.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/rom_bootstrap_generator.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/rom_bootstrap_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments_old.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments_old.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/sha256tree.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/sha256tree_module.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/sha256tree_module.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_launcher.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_launcher.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer_v1_1.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer_v1_1.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_truths.clib
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/tails.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/test_generator_deserialize.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/test_generator_deserialize.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/test_multiple_generator_input_arguments.clsp
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/test_multiple_generator_input_arguments.clsp.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/puzzles/utility_macros.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/secret_key_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/sign_coin_spends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43570 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/trade_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/trade_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.403016 chia-blockchain-1.8.0rc1/chia/wallet/trading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/trading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32738 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/trading/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/trading/trade_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/trading/trade_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/transaction_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/transaction_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/uncurried_puzzle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.407016 chia-blockchain-1.8.0rc1/chia/wallet/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/address_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/compute_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/compute_memos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/curry_and_treehash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/debug_spend_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/json_clvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/merkle_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/merkle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/new_peak_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/peer_request_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/puzzle_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17157 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/wallet_sync_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/util/wallet_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27732 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_coin_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_interested_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_nft_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79538 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_node_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_pool_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_puzzle_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_retry_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85610 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_transaction_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_user_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/chia/wallet/wallet_weight_proof_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.407016 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-20 03:20:39.000000 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32249 2023-04-20 03:20:39.000000 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 03:20:39.000000 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 03:20:39.000000 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 03:15:35.000000 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-20 03:20:39.000000 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 03:20:39.000000 chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6676 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/install-gui.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4910 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/install-plotter.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/install-timelord.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12552 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/installhelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.407016 chia-blockchain-1.8.0rc1/mozilla-ca/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:10.000000 chia-blockchain-1.8.0rc1/mozilla-ca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216583 2023-04-20 03:15:10.000000 chia-blockchain-1.8.0rc1/mozilla-ca/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/run-py-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 03:20:39.447016 chia-blockchain-1.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/start-gui.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.411016 chia-blockchain-1.8.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.411016 chia-blockchain-1.8.0rc1/tests/blockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/blockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/blockchain/blockchain_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/blockchain/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166834 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/blockchain/test_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37614 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/blockchain/test_blockchain_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2431 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/build-init-files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/build-job-matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/check_pytest_monitor_output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2398 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/check_sql_statements.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1750 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/chia-start-sim
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.411016 chia-blockchain-1.8.0rc1/tests/clvm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/benchmark_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_chialisp_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_clvm_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_curry_and_treehash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_puzzle_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_puzzle_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_serialized_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/clvm/test_spend_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.411016 chia-blockchain-1.8.0rc1/tests/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/cmds/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/cmds/test_wallet_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28635 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/connection_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.415016 chia-blockchain-1.8.0rc1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.415016 chia-blockchain-1.8.0rc1/tests/core/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/cmds/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/cmds/test_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38994 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/cmds/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/cmds/test_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.415016 chia-blockchain-1.8.0rc1/tests/core/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/consensus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/consensus/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/consensus/test_pot_iterations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.415016 chia-blockchain-1.8.0rc1/tests/core/custom_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/custom_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/custom_types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/custom_types/test_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/custom_types/test_proof_of_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/custom_types/test_spend_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.415016 chia-blockchain-1.8.0rc1/tests/core/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/daemon/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/daemon/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/daemon/test_daemon_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/daemon/test_keychain_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.419016 chia-blockchain-1.8.0rc1/tests/core/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_layer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245364 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47306 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_store_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/data_layer/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.419016 chia-blockchain-1.8.0rc1/tests/core/full_node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.419016 chia-blockchain-1.8.0rc1/tests/core/full_node/dos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/dos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/dos/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.419016 chia-blockchain-1.8.0rc1/tests/core/full_node/full_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/full_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/full_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/full_sync/test_full_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/ram_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.419016 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34130 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_full_node_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_hint_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_sync_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_address_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_block_height_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87563 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_full_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_generator_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_hint_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_node_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_peer_store_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/full_node/test_tx_processing_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187863 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/large_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/make_block_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.423016 chia-blockchain-1.8.0rc1/tests/core/mempool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/mempool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/mempool/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123916 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_fee_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_fee_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/node_height.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.423016 chia-blockchain-1.8.0rc1/tests/core/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/flood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/test_dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/test_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/test_rate_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/server/test_upnp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.423016 chia-blockchain-1.8.0rc1/tests/core/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/ssl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/ssl/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_coins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_cost_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_crawler_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_daemon_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_db_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_db_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23550 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_farmer_harvester_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_full_node_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_merkle_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/test_setproctitle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.423016 chia-blockchain-1.8.0rc1/tests/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_cached_bls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_file_keyring_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_jsonify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20681 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22952 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_keyring_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_significant_bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/core/util/test_streamable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.427016 chia-blockchain-1.8.0rc1/tests/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/db/test_db_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.427016 chia-blockchain-1.8.0rc1/tests/farmer_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/farmer_harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/farmer_harvester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/farmer_harvester/test_farmer_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.427016 chia-blockchain-1.8.0rc1/tests/fee_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/fee_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/fee_estimation/cmdline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/fee_estimation/test_fee_estimation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/fee_estimation/test_fee_estimation_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/fee_estimation/test_fee_estimation_unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/fee_estimation/test_mempoolitem_height_added.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.427016 chia-blockchain-1.8.0rc1/tests/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/generator/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/generator/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/generator/test_generator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/generator/test_list_to_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/generator/test_rom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/generator/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.427016 chia-blockchain-1.8.0rc1/tests/plot_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29365 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/test_plot_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/test_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/test_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/test_sync_simulated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plot_sync/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.427016 chia-blockchain-1.8.0rc1/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plotting/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32802 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plotting/test_plot_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/plotting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.431016 chia-blockchain-1.8.0rc1/tests/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/test_pool_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/test_pool_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/test_pool_puzzles_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47244 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/test_pool_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/test_pool_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/pools/test_wallet_pool_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.431016 chia-blockchain-1.8.0rc1/tests/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/simulation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/simulation/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/simulation/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/simulation/test_start_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/testconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.431016 chia-blockchain-1.8.0rc1/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/1315537.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/1315544.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/1315630.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/300000.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/442734.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233251 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/466212.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   405504 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/test-blockchain-db.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/test_full_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/test_legacy_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/tools/test_run_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.435016 chia-blockchain-1.8.0rc1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/alert_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/benchmark_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/bip39_test_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/build_network_protocol_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/gen_ssl_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/generator_tools_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/key_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/network_protocol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/protocol_messages_bytes-v1.0
+-rw-r--r--   0 runner    (1001) docker     (123)   170660 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/protocol_messages_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/temp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_full_block_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_limited_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_lock_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22379 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_network_protocol_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_network_protocol_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_network_protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_struct_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/util/test_trusted_peer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.439016 chia-blockchain-1.8.0rc1/tests/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.439016 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25164 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_cat_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_cat_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39540 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_cat_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_offer_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162923 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.439016 chia-blockchain-1.8.0rc1/tests/wallet/dao_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/dao_wallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.439016 chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/test_db_graftroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135852 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/test_dl_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/test_dl_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.439016 chia-blockchain-1.8.0rc1/tests/wallet/did_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/did_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/did_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65884 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/did_wallet/test_did.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.443016 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   374078 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_1_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43345 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_bulk_mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66774 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76327 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.443016 chia-blockchain-1.8.0rc1/tests/wallet/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/rpc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/rpc/test_dl_wallet_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74646 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/rpc/test_wallet_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.443016 chia-blockchain-1.8.0rc1/tests/wallet/simple_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/simple_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/simple_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/simple_sync/test_simple_sync_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.443016 chia-blockchain-1.8.0rc1/tests/wallet/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65909 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/sync/test_wallet_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_address_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_bech32m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_chialisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_coin_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_nft_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_offer_parsing_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_puzzle_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_singleton_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_singleton_lifecycle_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_taproot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28752 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_transaction_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43806 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_interested_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_key_val_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_trade_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_user_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.443016 chia-blockchain-1.8.0rc1/tests/weight_proof/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/weight_proof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/weight_proof/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tests/weight_proof/test_weight_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:20:39.447016 chia-blockchain-1.8.0rc1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5772 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/analyze-chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/analyze_memory_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/cpu_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/generate_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/legacy_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/manage_clvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/plot-log.gnuplot
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/run_benchmark.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/run_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/test_constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13441 2023-04-20 03:15:02.000000 chia-blockchain-1.8.0rc1/tools/test_full_sync.py
```

### Comparing `chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chia-blockchain-1.8.0rc1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/config.yml` & `chia-blockchain-1.8.0rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/PULL_REQUEST_TEMPLATE.md` & `chia-blockchain-1.8.0rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/actions/install/action.yml` & `chia-blockchain-1.8.0rc1/.github/actions/install/action.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/dependabot.yml` & `chia-blockchain-1.8.0rc1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/benchmarks.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/build-linux-arm64-installer.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/build-linux-arm64-installer.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-deb.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/build-linux-installer-deb.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-rpm.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/build-linux-installer-rpm.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/build-macos-installers.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/build-macos-installers.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/build-windows-installer.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/build-windows-installer.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/check-commit-signing.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/check-commit-signing.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/check_wheel_availability.yaml` & `chia-blockchain-1.8.0rc1/.github/workflows/check_wheel_availability.yaml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/codeql-analysis.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/conflict-check.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/conflict-check.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/dependency-review.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/mozilla-ca-cert.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/mozilla-ca-cert.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/pre-commit.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/require-labels.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/require-labels.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/snyk-python-scan.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/snyk-python-scan.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/stale-issue.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/start-release.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/start-release.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/start-sync-test.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/start-sync-test.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/super-linter.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/super-linter.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/test-install-scripts.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/test-install-scripts.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/test-single.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/test-single.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/test.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-dev.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/trigger-docker-dev.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-main.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/trigger-docker-main.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.github/workflows/upload-pypi-source.yml` & `chia-blockchain-1.8.0rc1/.github/workflows/upload-pypi-source.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.gitignore` & `chia-blockchain-1.8.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.markdown-lint.yml` & `chia-blockchain-1.8.0rc1/.markdown-lint.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/.pre-commit-config.yaml` & `chia-blockchain-1.8.0rc1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     hooks:
     -   id: black
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
-        exclude: ".*?(.hex|.clvm|.clib)"
+        exclude: ".*?(.hex|.clsp|.clvm|.clib)"
     -   id: trailing-whitespace
     -   id: check-merge-conflict
     -   id: check-ast
     -   id: debug-statements
 -   repo: local
     hooks:
     -   id: clvm_hex
-        name: .clvm.hex files
+        name: .clsp.hex files
         entry: ./activated.py python tools/manage_clvm.py check
         language: python
         pass_filenames: false
 -   repo: local
     hooks:
     -   id: mypy
         name: mypy
```

### Comparing `chia-blockchain-1.8.0b6/BUILD_TIMELORD.md` & `chia-blockchain-1.8.0rc1/BUILD_TIMELORD.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/CHANGELOG.md` & `chia-blockchain-1.8.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/CODE_OF_CONDUCT.md` & `chia-blockchain-1.8.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/CONTRIBUTING.md` & `chia-blockchain-1.8.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/Install-gui.ps1` & `chia-blockchain-1.8.0rc1/Install-gui.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/Install-plotter.ps1` & `chia-blockchain-1.8.0rc1/Install-plotter.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/Install.ps1` & `chia-blockchain-1.8.0rc1/Install.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/LICENSE` & `chia-blockchain-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/PKG-INFO` & `chia-blockchain-1.8.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia-blockchain
-Version: 1.8.0b6
+Version: 1.8.0rc1
 Summary: Chia blockchain full node, farmer, timelord, and wallet.
 Home-page: https://chia.net/
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Project-URL: Source, https://github.com/Chia-Network/chia-blockchain/
 Project-URL: Changelog, https://github.com/Chia-Network/chia-blockchain/blob/main/CHANGELOG.md
```

### Comparing `chia-blockchain-1.8.0b6/PRETTY_GOOD_PRACTICES.md` & `chia-blockchain-1.8.0rc1/PRETTY_GOOD_PRACTICES.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/README.md` & `chia-blockchain-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/SECURITY.md` & `chia-blockchain-1.8.0rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/activated.py` & `chia-blockchain-1.8.0rc1/activated.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/block_ref.py` & `chia-blockchain-1.8.0rc1/benchmarks/block_ref.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/block_store.py` & `chia-blockchain-1.8.0rc1/benchmarks/block_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/clvm_generator.bin` & `chia-blockchain-1.8.0rc1/benchmarks/clvm_generator.bin`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/coin_store.py` & `chia-blockchain-1.8.0rc1/benchmarks/coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/jsonify.py` & `chia-blockchain-1.8.0rc1/benchmarks/jsonify.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/mempool-long-lived.py` & `chia-blockchain-1.8.0rc1/benchmarks/mempool-long-lived.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/mempool.py` & `chia-blockchain-1.8.0rc1/benchmarks/mempool.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/streamable.py` & `chia-blockchain-1.8.0rc1/benchmarks/streamable.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/transaction_height_delta` & `chia-blockchain-1.8.0rc1/benchmarks/transaction_height_delta`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/benchmarks/utils.py` & `chia-blockchain-1.8.0rc1/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/assets/dmg/background.tiff` & `chia-blockchain-1.8.0rc1/build_scripts/assets/dmg/background.tiff`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-1-gui.sh` & `chia-blockchain-1.8.0rc1/build_scripts/build_linux_deb-1-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-2-installer.sh` & `chia-blockchain-1.8.0rc1/build_scripts/build_linux_deb-2-installer.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-1-gui.sh` & `chia-blockchain-1.8.0rc1/build_scripts/build_linux_rpm-1-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-2-installer.sh` & `chia-blockchain-1.8.0rc1/build_scripts/build_linux_rpm-2-installer.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_macos-1-gui.sh` & `chia-blockchain-1.8.0rc1/build_scripts/build_macos-1-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_macos-2-installer.sh` & `chia-blockchain-1.8.0rc1/build_scripts/build_macos-2-installer.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_windows-1-gui.ps1` & `chia-blockchain-1.8.0rc1/build_scripts/build_windows-1-gui.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/build_windows-2-installer.ps1` & `chia-blockchain-1.8.0rc1/build_scripts/build_windows-2-installer.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/check_dependency_artifacts.py` & `chia-blockchain-1.8.0rc1/build_scripts/check_dependency_artifacts.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/clean-runner.sh` & `chia-blockchain-1.8.0rc1/build_scripts/clean-runner.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/installer-version.py` & `chia-blockchain-1.8.0rc1/build_scripts/installer-version.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/npm_linux/package-lock.json` & `chia-blockchain-1.8.0rc1/build_scripts/npm_linux/package-lock.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/npm_macos/package-lock.json` & `chia-blockchain-1.8.0rc1/build_scripts/npm_macos/package-lock.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/build_scripts/npm_windows/package-lock.json` & `chia-blockchain-1.8.0rc1/build_scripts/npm_windows/package-lock.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/clvm/spend_sim.py` & `chia-blockchain-1.8.0rc1/chia/clvm/spend_sim.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/beta.py` & `chia-blockchain-1.8.0rc1/chia/cmds/beta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/beta_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/beta_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/check_wallet_db.py` & `chia-blockchain-1.8.0rc1/chia/cmds/check_wallet_db.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/chia.py` & `chia-blockchain-1.8.0rc1/chia/cmds/chia.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from chia import __version__
 from chia.cmds.beta import beta_cmd
 from chia.cmds.completion import completion
 from chia.cmds.configure import configure_cmd
 from chia.cmds.data import data_cmd
 from chia.cmds.db import db_cmd
+from chia.cmds.dev import dev_cmd
 from chia.cmds.farm import farm_cmd
 from chia.cmds.init import init_cmd
 from chia.cmds.keys import keys_cmd
 from chia.cmds.netspace import netspace_cmd
 from chia.cmds.passphrase import passphrase_cmd
 from chia.cmds.peer import peer_cmd
 from chia.cmds.plotnft import plotnft_cmd
@@ -123,14 +124,15 @@
 cli.add_command(plotters_cmd)
 cli.add_command(db_cmd)
 cli.add_command(peer_cmd)
 cli.add_command(data_cmd)
 cli.add_command(passphrase_cmd)
 cli.add_command(beta_cmd)
 cli.add_command(completion)
+cli.add_command(dev_cmd)
 
 
 def main() -> None:
     cli()  # pylint: disable=no-value-for-parameter
 
 
 if __name__ == "__main__":
```

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/cmds_util.py` & `chia-blockchain-1.8.0rc1/chia/cmds/cmds_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,36 +11,39 @@
 from chia.daemon.keychain_proxy import KeychainProxy, connect_to_keychain_and_validate
 from chia.rpc.data_layer_rpc_client import DataLayerRpcClient
 from chia.rpc.farmer_rpc_client import FarmerRpcClient
 from chia.rpc.full_node_rpc_client import FullNodeRpcClient
 from chia.rpc.harvester_rpc_client import HarvesterRpcClient
 from chia.rpc.rpc_client import RpcClient
 from chia.rpc.wallet_rpc_client import WalletRpcClient
+from chia.simulator.simulator_full_node_rpc_client import SimulatorFullNodeRpcClient
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.mempool_submission_status import MempoolSubmissionStatus
 from chia.util.config import load_config
 from chia.util.default_root import DEFAULT_ROOT_PATH
 from chia.util.ints import uint16
 from chia.util.keychain import KeyData
 from chia.wallet.transaction_record import TransactionRecord
 
 NODE_TYPES: Dict[str, Type[RpcClient]] = {
     "farmer": FarmerRpcClient,
     "wallet": WalletRpcClient,
     "full_node": FullNodeRpcClient,
     "harvester": HarvesterRpcClient,
     "data_layer": DataLayerRpcClient,
+    "simulator": SimulatorFullNodeRpcClient,
 }
 
 node_config_section_names: Dict[Type[RpcClient], str] = {
     FarmerRpcClient: "farmer",
     WalletRpcClient: "wallet",
     FullNodeRpcClient: "full_node",
     HarvesterRpcClient: "harvester",
     DataLayerRpcClient: "data_layer",
+    SimulatorFullNodeRpcClient: "full_node",
 }
 
 
 _T_RpcClient = TypeVar("_T_RpcClient", bound=RpcClient)
 
 
 def transaction_submitted_msg(tx: TransactionRecord) -> str:
@@ -55,36 +58,40 @@
 async def validate_client_connection(
     rpc_client: RpcClient,
     node_type: str,
     rpc_port: int,
     root_path: Path,
     fingerprint: Optional[int],
     login_to_wallet: bool,
-) -> Optional[int]:
+    consume_errors: bool = True,
+) -> Tuple[Optional[int], bool]:
+    connected: bool = True
     try:
         await rpc_client.healthz()
         if type(rpc_client) == WalletRpcClient and login_to_wallet:
             fingerprint = await get_wallet(root_path, rpc_client, fingerprint)
             if fingerprint is None:
-                rpc_client.close()
+                connected = False
     except ClientConnectorError:
+        if not consume_errors:
+            raise
+        connected = False
         print(f"Connection error. Check if {node_type.replace('_', ' ')} rpc is running at {rpc_port}")
         print(f"This is normal if {node_type.replace('_', ' ')} is still starting up")
-        rpc_client.close()
-    await rpc_client.await_closed()  # if close is not already called this does nothing
-    return fingerprint
+    return fingerprint, connected
 
 
 @asynccontextmanager
 async def get_any_service_client(
     client_type: Type[_T_RpcClient],
     rpc_port: Optional[int] = None,
     root_path: Path = DEFAULT_ROOT_PATH,
     fingerprint: Optional[int] = None,
     login_to_wallet: bool = True,
+    consume_errors: bool = True,
 ) -> AsyncIterator[Tuple[Optional[_T_RpcClient], Dict[str, Any], Optional[int]]]:
     """
     Yields a tuple with a RpcClient for the applicable node type a dictionary of the node's configuration,
     and a fingerprint if applicable. However, if connecting to the node fails then we will return None for
     the RpcClient.
     """
 
@@ -97,23 +104,25 @@
     self_hostname = config["self_hostname"]
     if rpc_port is None:
         rpc_port = config[node_type]["rpc_port"]
     # select node client type based on string
     node_client = await client_type.create(self_hostname, uint16(rpc_port), root_path, config)
     try:
         # check if we can connect to node, and if we can then validate
-        # fingerprint access, otherwise return fingerprint and shutdown client
-        fingerprint = await validate_client_connection(
-            node_client, node_type, rpc_port, root_path, fingerprint, login_to_wallet
+        # fingerprint access (if wallet), otherwise return fingerprint and set connected to False
+        fingerprint, connected = await validate_client_connection(
+            node_client, node_type, rpc_port, root_path, fingerprint, login_to_wallet, consume_errors
         )
-        if node_client.session.closed:
-            yield None, config, fingerprint
-        else:
+        if connected:
             yield node_client, config, fingerprint
+        else:
+            yield None, config, fingerprint
     except Exception as e:  # this is only here to make the errors more user-friendly.
+        if not consume_errors:
+            raise
         print(f"Exception from '{node_type}' {e}:\n{traceback.format_exc()}")
 
     finally:
         node_client.close()  # this can run even if already closed, will just do nothing.
         await node_client.await_closed()
```

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/coin_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/coin_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/coins.py` & `chia-blockchain-1.8.0rc1/chia/cmds/coins.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/completion.py` & `chia-blockchain-1.8.0rc1/chia/cmds/completion.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/configure.py` & `chia-blockchain-1.8.0rc1/chia/cmds/configure.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/data.py` & `chia-blockchain-1.8.0rc1/chia/cmds/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -383,7 +383,22 @@
 def get_sync_status(
     id: str,
     data_rpc_port: int,
 ) -> None:
     from chia.cmds.data_funcs import get_sync_status_cmd
 
     run(get_sync_status_cmd(rpc_port=data_rpc_port, store_id=id))
+
+
+@data_cmd.group("plugins", help="Get information about configured uploader/downloader plugins")
+def plugins_cmd() -> None:
+    pass
+
+
+@plugins_cmd.command("check", help="Calls the plugin_info endpoint on all configured plugins")
+@create_rpc_port_option()
+def check_plugins(
+    data_rpc_port: int,
+) -> None:
+    from chia.cmds.data_funcs import check_plugins_cmd
+
+    run(check_plugins_cmd(rpc_port=data_rpc_port))
```

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/data_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/data_funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import json
 from decimal import Decimal
 from pathlib import Path
 from typing import Dict, List, Optional
 
 from chia.cmds.cmds_util import get_any_service_client
 from chia.cmds.units import units
 from chia.rpc.data_layer_rpc_client import DataLayerRpcClient
@@ -210,7 +211,14 @@
     store_id: str,
 ) -> None:
     store_id_bytes = bytes32.from_hexstr(store_id)
     async with get_any_service_client(DataLayerRpcClient, rpc_port) as (client, _, _):
         if client is not None:
             res = await client.get_sync_status(store_id=store_id_bytes)
             print(res)
+
+
+async def check_plugins_cmd(rpc_port: Optional[int]) -> None:
+    async with get_any_service_client(DataLayerRpcClient, rpc_port) as (client, _, _):
+        if client is not None:
+            res = await client.check_plugins()
+            print(json.dumps(res, indent=4, sort_keys=True))
```

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/db.py` & `chia-blockchain-1.8.0rc1/chia/cmds/db.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/db_backup_func.py` & `chia-blockchain-1.8.0rc1/chia/cmds/db_backup_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/db_upgrade_func.py` & `chia-blockchain-1.8.0rc1/chia/cmds/db_upgrade_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/db_validate_func.py` & `chia-blockchain-1.8.0rc1/chia/cmds/db_validate_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/farm.py` & `chia-blockchain-1.8.0rc1/chia/cmds/farm.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/farm_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/farm_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/init.py` & `chia-blockchain-1.8.0rc1/chia/cmds/init.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/init_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/init_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/keys.py` & `chia-blockchain-1.8.0rc1/chia/cmds/keys.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/keys_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/keys_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/netspace.py` & `chia-blockchain-1.8.0rc1/chia/cmds/netspace.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/netspace_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/netspace_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/passphrase.py` & `chia-blockchain-1.8.0rc1/chia/cmds/passphrase.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/passphrase_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/passphrase_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/peer.py` & `chia-blockchain-1.8.0rc1/chia/cmds/peer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/peer_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/peer_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/plotnft.py` & `chia-blockchain-1.8.0rc1/chia/cmds/plotnft.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/plotnft_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/plotnft_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/plots.py` & `chia-blockchain-1.8.0rc1/chia/cmds/plots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/rpc.py` & `chia-blockchain-1.8.0rc1/chia/cmds/rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/show.py` & `chia-blockchain-1.8.0rc1/chia/cmds/show.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/show_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/show_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/start.py` & `chia-blockchain-1.8.0rc1/chia/cmds/start.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from chia.util.service_groups import all_groups
 
 
 @click.command("start", short_help="Start service groups")
 @click.option("-r", "--restart", is_flag=True, type=bool, help="Restart running services")
 @click.argument("group", type=click.Choice(list(all_groups())), nargs=-1, required=True)
 @click.pass_context
-def start_cmd(ctx: click.Context, restart: bool, group: str) -> None:
+def start_cmd(ctx: click.Context, restart: bool, group: tuple[str, ...]) -> None:
     import asyncio
 
     from chia.cmds.beta_funcs import warn_if_beta_enabled
 
     from .start_funcs import async_start
 
     root_path = ctx.obj["root_path"]
```

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/start_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/start_funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             print("Unlocking daemon keyring")
             await connection.unlock_keyring(passphrase)
 
         return connection
     return None
 
 
-async def async_start(root_path: Path, config: Dict[str, Any], group: str, restart: bool) -> None:
+async def async_start(root_path: Path, config: Dict[str, Any], group: tuple[str, ...], restart: bool) -> None:
     try:
         daemon = await create_start_daemon_connection(root_path, config)
     except KeychainMaxUnlockAttempts:
         print("Failed to unlock keyring")
         return None
 
     if daemon is None:
```

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/stop.py` & `chia-blockchain-1.8.0rc1/chia/cmds/stop.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import click
 
 from chia.util.config import load_config
 from chia.util.service_groups import all_groups, services_for_groups
 
 
-async def async_stop(root_path: Path, config: Dict[str, Any], group: str, stop_daemon: bool) -> int:
+async def async_stop(root_path: Path, config: Dict[str, Any], group: tuple[str, ...], stop_daemon: bool) -> int:
     from chia.daemon.client import connect_to_daemon_and_validate
 
     daemon = await connect_to_daemon_and_validate(root_path, config)
     if daemon is None:
         print("Couldn't connect to chia daemon")
         return 1
 
@@ -47,15 +47,15 @@
     return return_val
 
 
 @click.command("stop", short_help="Stop services")
 @click.option("-d", "--daemon", is_flag=True, type=bool, help="Stop daemon")
 @click.argument("group", type=click.Choice(list(all_groups())), nargs=-1, required=True)
 @click.pass_context
-def stop_cmd(ctx: click.Context, daemon: bool, group: str) -> None:
+def stop_cmd(ctx: click.Context, daemon: bool, group: tuple[str, ...]) -> None:
     from chia.cmds.beta_funcs import warn_if_beta_enabled
 
     root_path = ctx.obj["root_path"]
     config = load_config(root_path, "config.yaml")
     warn_if_beta_enabled(config)
 
     sys.exit(asyncio.run(async_stop(root_path, config, group, daemon)))
```

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/wallet.py` & `chia-blockchain-1.8.0rc1/chia/cmds/wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/cmds/wallet_funcs.py` & `chia-blockchain-1.8.0rc1/chia/cmds/wallet_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,24 +458,26 @@
                     print("Not creating offer...")
                     return
 
             confirmation = input("Confirm (y/n): ")
             if confirmation not in ["y", "yes"]:
                 print("Not creating offer...")
             else:
-                offer, trade_record = await wallet_client.create_offer_for_ids(
-                    offer_dict, driver_dict=driver_dict, fee=fee, reuse_puzhash=reuse_puzhash
-                )
-                if offer is not None:
-                    with open(pathlib.Path(filepath), "w") as file:
+                with open(pathlib.Path(filepath), "w") as file:
+                    offer, trade_record = await wallet_client.create_offer_for_ids(
+                        offer_dict, driver_dict=driver_dict, fee=fee, reuse_puzhash=reuse_puzhash
+                    )
+                    if offer is not None:
                         file.write(offer.to_bech32())
-                    print(f"Created offer with ID {trade_record.trade_id}")
-                    print(f"Use chia wallet get_offers --id {trade_record.trade_id} -f {fingerprint} to view status")
-                else:
-                    print("Error creating offer")
+                        print(f"Created offer with ID {trade_record.trade_id}")
+                        print(
+                            f"Use chia wallet get_offers --id {trade_record.trade_id} -f {fingerprint} to view status"
+                        )
+                    else:
+                        print("Error creating offer")
 
 
 def timestamp_to_time(timestamp):
     return datetime.fromtimestamp(timestamp).strftime("%Y-%m-%d %H:%M:%S")
 
 
 async def print_offer_summary(cat_name_resolver: CATNameResolver, sum_dict: Dict[str, int], has_fee: bool = False):
```

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/block_body_validation.py` & `chia-blockchain-1.8.0rc1/chia/consensus/block_body_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/block_creation.py` & `chia-blockchain-1.8.0rc1/chia/consensus/block_creation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/block_header_validation.py` & `chia-blockchain-1.8.0rc1/chia/consensus/block_header_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/block_record.py` & `chia-blockchain-1.8.0rc1/chia/consensus/block_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/block_rewards.py` & `chia-blockchain-1.8.0rc1/chia/consensus/block_rewards.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/block_root_validation.py` & `chia-blockchain-1.8.0rc1/chia/consensus/block_root_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/blockchain.py` & `chia-blockchain-1.8.0rc1/chia/consensus/blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/blockchain_interface.py` & `chia-blockchain-1.8.0rc1/chia/consensus/blockchain_interface.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/coinbase.py` & `chia-blockchain-1.8.0rc1/chia/consensus/coinbase.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/constants.py` & `chia-blockchain-1.8.0rc1/chia/consensus/constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/cost_calculator.py` & `chia-blockchain-1.8.0rc1/chia/consensus/cost_calculator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/default_constants.py` & `chia-blockchain-1.8.0rc1/chia/consensus/default_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/deficit.py` & `chia-blockchain-1.8.0rc1/chia/consensus/deficit.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/difficulty_adjustment.py` & `chia-blockchain-1.8.0rc1/chia/consensus/difficulty_adjustment.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/find_fork_point.py` & `chia-blockchain-1.8.0rc1/chia/consensus/find_fork_point.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/full_block_to_block_record.py` & `chia-blockchain-1.8.0rc1/chia/consensus/full_block_to_block_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/get_block_challenge.py` & `chia-blockchain-1.8.0rc1/chia/consensus/get_block_challenge.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/make_sub_epoch_summary.py` & `chia-blockchain-1.8.0rc1/chia/consensus/make_sub_epoch_summary.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/multiprocess_validation.py` & `chia-blockchain-1.8.0rc1/chia/consensus/multiprocess_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/pos_quality.py` & `chia-blockchain-1.8.0rc1/chia/consensus/pos_quality.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/pot_iterations.py` & `chia-blockchain-1.8.0rc1/chia/consensus/pot_iterations.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/consensus/vdf_info_computation.py` & `chia-blockchain-1.8.0rc1/chia/consensus/vdf_info_computation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/daemon/client.py` & `chia-blockchain-1.8.0rc1/chia/daemon/client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/daemon/keychain_proxy.py` & `chia-blockchain-1.8.0rc1/chia/daemon/keychain_proxy.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/daemon/keychain_server.py` & `chia-blockchain-1.8.0rc1/chia/daemon/keychain_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/daemon/server.py` & `chia-blockchain-1.8.0rc1/chia/daemon/server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/daemon/windows_signal.py` & `chia-blockchain-1.8.0rc1/chia/daemon/windows_signal.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/data_layer.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/data_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import json
 import logging
 import os
 import random
 import time
 import traceback
 from pathlib import Path
 from typing import Any, Awaitable, Dict, List, Optional, Set, Tuple, Union
@@ -15,14 +16,15 @@
 from chia.data_layer.data_layer_util import (
     DiffData,
     InternalNode,
     KeyValue,
     Layer,
     Offer,
     OfferStore,
+    PluginStatus,
     Proof,
     ProofOfInclusion,
     ProofOfInclusionLayer,
     Root,
     ServerInfo,
     Status,
     StoreProofs,
@@ -43,14 +45,26 @@
 from chia.util.ints import uint32, uint64
 from chia.util.path import path_from_root
 from chia.wallet.trade_record import TradeRecord
 from chia.wallet.trading.offer import Offer as TradingOffer
 from chia.wallet.transaction_record import TransactionRecord
 
 
+async def get_plugin_info(url: str) -> Tuple[str, Dict[str, Any]]:
+    try:
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url + "/plugin_info", json={}) as response:
+                ret = {"status": response.status}
+                if response.status == 200:
+                    ret["response"] = json.loads(await response.text())
+                return url, ret
+    except aiohttp.ClientError as e:
+        return url, {"error": f"ClientError: {e}"}
+
+
 class DataLayer:
     data_store: DataStore
     db_path: Path
     config: Dict[str, Any]
     log: logging.Logger
     wallet_rpc_init: Awaitable[WalletRpcClient]
     state_changed_callback: Optional[StateChangedProtocol] = None
@@ -438,22 +452,22 @@
         publish_generation = min(singleton_record.generation, 0 if root is None else root.generation)
         # If we make some batch updates, which get confirmed to the chain, we need to create the files.
         # We iterate back and write the missing files, until we find the files already written.
         root = await self.data_store.get_tree_root(tree_id=tree_id, generation=publish_generation)
         while publish_generation > 0:
             write_file_result = await write_files_for_root(self.data_store, tree_id, root, self.server_files_location)
             if not write_file_result.result:
-                self.log.error("failed to write files")
+                # this particular return only happens if the files already exist, no need to log anything
                 break
             try:
                 if uploaders is not None and len(uploaders) > 0:
                     request_json = {
                         "store_id": tree_id.hex(),
-                        "full_tree_path": str(write_file_result.full_tree),
-                        "diff_path": str(write_file_result.diff_tree),
+                        "full_tree_filename": write_file_result.full_tree.name,
+                        "diff_filename": write_file_result.diff_tree.name,
                     }
                     for uploader in uploaders:
                         self.log.info(f"Using uploader {uploader} for store {tree_id.hex()}")
                         async with aiohttp.ClientSession() as session:
                             async with session.post(uploader + "/upload", json=request_json) as response:
                                 res_json = await response.json()
                                 if res_json["uploaded"]:
@@ -461,15 +475,14 @@
                                         f"Uploaded files to {uploader} for store {tree_id.hex()} "
                                         "generation {publish_generation}"
                                     )
                                 else:
                                     self.log.error(
                                         f"Failed to upload files to, will retry later: {uploader} : {res_json}"
                                     )
-                                    break  # todo this will retry all uploaders
             except Exception as e:
                 self.log.error(f"Exception uploading files, will retry later: tree id {tree_id}")
                 self.log.debug(f"Failed to upload files, cleaning local files: {type(e).__name__}: {e}")
                 os.remove(write_file_result.full_tree)
                 os.remove(write_file_result.diff_tree)
             publish_generation -= 1
             root = await self.data_store.get_tree_root(tree_id=tree_id, generation=publish_generation)
@@ -478,17 +491,32 @@
         root = await self.data_store.get_tree_root(tree_id=store_id)
         singleton_record: Optional[SingletonRecord] = await self.wallet_rpc.dl_latest_singleton(store_id, True)
         if singleton_record is None:
             self.log.error(f"No singleton record found for: {store_id}")
             return
         max_generation = min(singleton_record.generation, 0 if root is None else root.generation)
         server_files_location = foldername if foldername is not None else self.server_files_location
+        files = []
         for generation in range(1, max_generation + 1):
             root = await self.data_store.get_tree_root(tree_id=store_id, generation=generation)
-            await write_files_for_root(self.data_store, store_id, root, server_files_location, overwrite)
+            res = await write_files_for_root(self.data_store, store_id, root, server_files_location, overwrite)
+            files.append(res.diff_tree.name)
+            files.append(res.full_tree.name)
+
+        uploaders = await self.get_uploaders(store_id)
+        if uploaders is not None and len(uploaders) > 0:
+            request_json = {"store_id": store_id.hex(), "files": json.dumps(files)}
+            for uploader in uploaders:
+                async with aiohttp.ClientSession() as session:
+                    async with session.post(uploader + "/add_missing_files", json=request_json) as response:
+                        res_json = await response.json()
+                        if not res_json["uploaded"]:
+                            self.log.error(f"failed to upload to uploader {uploader}")
+                        else:
+                            self.log.debug(f"uploaded to uploader {uploader}")
 
     async def subscribe(self, store_id: bytes32, urls: List[str]) -> None:
         parsed_urls = [url.rstrip("/") for url in urls]
         subscription = Subscription(store_id, [ServerInfo(url, 0, 0) for url in parsed_urls])
         await self.wallet_rpc.dl_track_new(subscription.tree_id)
         async with self.subscription_lock:
             await self.data_store.subscribe(subscription)
@@ -859,7 +887,16 @@
                     async with session.post(uploader + "/handle_upload", json={"store_id": tree_id.hex()}) as response:
                         res_json = await response.json()
                         if res_json["handle_upload"]:
                             uploaders.append(uploader)
                 except Exception as e:
                     self.log.error(f"get_uploader could not get response {e}")
         return uploaders
+
+    async def check_plugins(self) -> PluginStatus:
+        coros = [get_plugin_info(url=plugin) for plugin in {*self.uploaders, *self.downloaders}]
+        results = dict(await asyncio.gather(*coros))
+
+        uploader_status = {url: results.get(url, "unknown") for url in self.uploaders}
+        downloader_status = {url: results.get(url, "unknown") for url in self.downloaders}
+
+        return PluginStatus(uploaders=uploader_status, downloaders=downloader_status)
```

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_api.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_errors.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_errors.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_server.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_util.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,7 +619,21 @@
 
 @dataclasses.dataclass(frozen=True)
 class SyncStatus:
     root_hash: bytes32
     generation: int
     target_root_hash: bytes32
     target_generation: int
+
+
+@dataclasses.dataclass(frozen=True)
+class PluginStatus:
+    uploaders: Dict[str, Dict[str, Any]]
+    downloaders: Dict[str, Dict[str, Any]]
+
+    def marshal(self) -> Dict[str, Any]:
+        return {
+            "plugin_status": {
+                "uploaders": self.uploaders,
+                "downloaders": self.downloaders,
+            }
+        }
```

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_wallet.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/data_layer_wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from chia.wallet.puzzles.singleton_top_layer_v1_1 import SINGLETON_LAUNCHER_HASH
 from chia.wallet.sign_coin_spends import sign_coin_spends
 from chia.wallet.trading.offer import NotarizedPayment, Offer
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.util.compute_memos import compute_memos
 from chia.wallet.util.merkle_utils import _simplify_merkle_proof
 from chia.wallet.util.transaction_type import TransactionType
+from chia.wallet.util.wallet_sync_utils import fetch_coin_spend, fetch_coin_spend_for_coin_state
 from chia.wallet.util.wallet_types import AmountWithPuzzlehash, WalletType
 from chia.wallet.wallet import Wallet
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_info import WalletInfo
 
 if TYPE_CHECKING:
     from chia.wallet.wallet_state_manager import WalletStateManager
@@ -213,17 +214,15 @@
         if await self.wallet_state_manager.dl_store.get_launcher(launcher_id) is not None:
             self.log.info(f"Spend of launcher {launcher_id} has already been processed")
             return None
         if spend is not None and spend.coin.name() == launcher_id:  # spend.coin.name() == launcher_id is a sanity check
             await self.new_launcher_spend(spend, peer, height)
         else:
             launcher_state: CoinState = await self.get_launcher_coin_state(launcher_id, peer)
-            launcher_spend: CoinSpend = await self.wallet_state_manager.wallet_node.fetch_puzzle_solution(
-                launcher_state.spent_height, launcher_state.coin, peer
-            )
+            launcher_spend = await fetch_coin_spend_for_coin_state(launcher_state, peer)
             await self.new_launcher_spend(launcher_spend, peer)
 
     async def new_launcher_spend(
         self,
         launcher_spend: CoinSpend,
         peer: WSChiaConnection,
         height: Optional[uint32] = None,
@@ -275,17 +274,15 @@
         await self.wallet_state_manager.add_interested_coin_ids([new_singleton.name()])
 
         new_singleton_coin_record: Optional[
             WalletCoinRecord
         ] = await self.wallet_state_manager.coin_store.get_coin_record(new_singleton.name())
         while new_singleton_coin_record is not None and new_singleton_coin_record.spent_block_height > 0:
             # We've already synced this before, so we need to sort of force a resync
-            parent_spend: CoinSpend = await self.wallet_state_manager.wallet_node.fetch_puzzle_solution(
-                new_singleton_coin_record.spent_block_height, new_singleton, peer
-            )
+            parent_spend = await fetch_coin_spend(new_singleton_coin_record.spent_block_height, new_singleton, peer)
             await self.singleton_removed(parent_spend, new_singleton_coin_record.spent_block_height)
             try:
                 additions = compute_additions(parent_spend)
                 new_singleton = next(coin for coin in additions if coin.amount % 2 != 0)
                 new_singleton_coin_record = await self.wallet_state_manager.coin_store.get_coin_record(
                     new_singleton.name()
                 )
@@ -825,17 +822,15 @@
     ###########
 
     async def coin_added(self, coin: Coin, height: uint32, peer: WSChiaConnection) -> None:
         if coin.puzzle_hash == create_mirror_puzzle().get_tree_hash():
             parent_state: CoinState = (
                 await self.wallet_state_manager.wallet_node.get_coin_state([coin.parent_coin_info], peer=peer)
             )[0]
-            parent_spend: Optional[CoinSpend] = await self.wallet_state_manager.wallet_node.fetch_puzzle_solution(
-                height, parent_state.coin, peer
-            )
+            parent_spend = await fetch_coin_spend(height, parent_state.coin, peer)
             assert parent_spend is not None
             launcher_id, urls = get_mirror_info(
                 parent_spend.puzzle_reveal.to_program(), parent_spend.solution.to_program()
             )
             if await self.wallet_state_manager.dl_store.is_launcher_tracked(launcher_id):
                 ours: bool = await self.wallet_state_manager.get_wallet_for_coin(coin.parent_coin_info) is not None
                 await self.wallet_state_manager.dl_store.add_mirror(
```

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/data_store.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/data_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/dl_wallet_store.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/dl_wallet_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/download_data.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/download_data.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/s3_plugin_config.yml` & `chia-blockchain-1.8.0rc1/chia/data_layer/s3_plugin_config.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 instance-1:
   log_filename: "s3_plugin.log"
+  log_level: INFO
+  server_files_location: "/Users/test/.chia/mainnet/data_layer/db/server_files_location_testnet10"
   port: 8998
   aws_credentials:
     access_key_id: "xxx"
     secret_access_key: "xxx"
     region: "xxx"
 
   stores:
@@ -12,14 +14,15 @@
       download_urls: ["s3://hello", "s3://goodbye"]
     - store_id: "a14daf55d41ced6419bcd011fbc1f74ab9567fe55340d88435aa6493d628fa47"
       upload_bucket:
       download_urls: ["s3://hello", "s3://goodbye"]
 
 instance-2:
   port: 8999
+  server_files_location: "/Users/test/.chia/mainnet/data_layer/db/server_files_location_testnet10"
   aws_credentials:
     access_key_id: "xxx"
     secret_access_key: "xxx"
     region: "xxx"
 
   stores:
     - store_id: "7acfcbd1ed73bfe2b698508f4ea5ed353c60ace154360272ce91f9ab0c8423c3"
```

### Comparing `chia-blockchain-1.8.0b6/chia/data_layer/util/benchmark.py` & `chia-blockchain-1.8.0rc1/chia/data_layer/util/benchmark.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/farmer/farmer.py` & `chia-blockchain-1.8.0rc1/chia/farmer/farmer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/farmer/farmer_api.py` & `chia-blockchain-1.8.0rc1/chia/farmer/farmer_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/bitcoin_fee_estimator.py` & `chia-blockchain-1.8.0rc1/chia/full_node/bitcoin_fee_estimator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/block_height_map.py` & `chia-blockchain-1.8.0rc1/chia/full_node/block_height_map.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/block_store.py` & `chia-blockchain-1.8.0rc1/chia/full_node/block_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/bundle_tools.py` & `chia-blockchain-1.8.0rc1/chia/full_node/bundle_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/coin_store.py` & `chia-blockchain-1.8.0rc1/chia/full_node/coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_estimate.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_estimate.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_estimate_store.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_estimate_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_estimation.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_estimation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_constants.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_example.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator_example.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_interface.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_estimator_interface.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_history.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_history.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/fee_tracker.py` & `chia-blockchain-1.8.0rc1/chia/full_node/fee_tracker.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/full_node.py` & `chia-blockchain-1.8.0rc1/chia/full_node/full_node.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/full_node_api.py` & `chia-blockchain-1.8.0rc1/chia/full_node/full_node_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/full_node_store.py` & `chia-blockchain-1.8.0rc1/chia/full_node/full_node_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/generator.py` & `chia-blockchain-1.8.0rc1/chia/full_node/generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from __future__ import annotations
 
 import logging
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.generator_types import BlockGenerator, CompressorArg, GeneratorBlockCacheInterface
 from chia.util.ints import uint32
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
-from chia.wallet.puzzles.rom_bootstrap_generator import get_generator
 
-GENERATOR_MOD = get_generator()
-
-DECOMPRESS_BLOCK = load_clvm_maybe_recompile("block_program_zero.clvm", package_or_requirement="chia.wallet.puzzles")
-DECOMPRESS_PUZZLE = load_clvm_maybe_recompile("decompress_puzzle.clvm", package_or_requirement="chia.wallet.puzzles")
+DECOMPRESS_BLOCK = load_clvm_maybe_recompile("block_program_zero.clsp", package_or_requirement="chia.wallet.puzzles")
+DECOMPRESS_PUZZLE = load_clvm_maybe_recompile("decompress_puzzle.clsp", package_or_requirement="chia.wallet.puzzles")
 # DECOMPRESS_CSE = load_clvm_maybe_recompile(
-#     "decompress_coin_spend_entry.clvm",
+#     "decompress_coin_spend_entry.clsp",
 #     package_or_requirement="chia.wallet.puzzles",
 # )
 
 DECOMPRESS_CSE_WITH_PREFIX = load_clvm_maybe_recompile(
-    "decompress_coin_spend_entry_with_prefix.clvm", package_or_requirement="chia.wallet.puzzles"
+    "decompress_coin_spend_entry_with_prefix.clsp", package_or_requirement="chia.wallet.puzzles"
 )
 log = logging.getLogger(__name__)
 
 
 def create_block_generator(
     generator: SerializedProgram, block_heights_list: List[uint32], generator_block_cache: GeneratorBlockCacheInterface
 ) -> Optional[BlockGenerator]:
@@ -37,46 +34,21 @@
             log.error(f"Failed to look up generator for block {i}. Ref List: {block_heights_list}")
             return None
         generator_list.append(previous_generator)
         generator_heights.append(i)
     return BlockGenerator(generator, generator_list, generator_heights)
 
 
-def create_generator_args(generator_ref_list: List[SerializedProgram]) -> Program:
-    """
-    `create_generator_args`: The format and contents of these arguments affect consensus.
-    """
-    gen_ref_list = [bytes(g) for g in generator_ref_list]
-    ret: Program = Program.to([gen_ref_list])
-    return ret
-
-
 def create_compressed_generator(
     original_generator: CompressorArg,
     compressed_cse_list: List[List[List[Union[bytes, None, int, Program]]]],
 ) -> BlockGenerator:
     """
     Bind the generator block program template to a particular reference block,
     template bytes offsets, and SpendBundle.
     """
     start = original_generator.start
     end = original_generator.end
     program = DECOMPRESS_BLOCK.curry(
         DECOMPRESS_PUZZLE, DECOMPRESS_CSE_WITH_PREFIX, Program.to(start), Program.to(end), compressed_cse_list
     )
     return BlockGenerator(program, [original_generator.generator], [original_generator.block_height])
-
-
-def setup_generator_args(self: BlockGenerator) -> Tuple[SerializedProgram, Program]:
-    args = create_generator_args(self.generator_refs)
-    return self.program, args
-
-
-def run_generator_mempool(self: BlockGenerator, max_cost: int) -> Tuple[int, SerializedProgram]:
-    program, args = setup_generator_args(self)
-    return GENERATOR_MOD.run_mempool_with_cost(max_cost, program, args)
-
-
-def run_generator_unsafe(self: BlockGenerator, max_cost: int) -> Tuple[int, SerializedProgram]:
-    """This mode is meant for accepting possibly soft-forked transactions into the mempool"""
-    program, args = setup_generator_args(self)
-    return GENERATOR_MOD.run_with_cost(max_cost, program, args)
```

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/hint_management.py` & `chia-blockchain-1.8.0rc1/chia/full_node/hint_management.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/hint_store.py` & `chia-blockchain-1.8.0rc1/chia/full_node/hint_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/lock_queue.py` & `chia-blockchain-1.8.0rc1/chia/full_node/lock_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/mempool.py` & `chia-blockchain-1.8.0rc1/chia/full_node/mempool.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/mempool_check_conditions.py` & `chia-blockchain-1.8.0rc1/chia/full_node/mempool_check_conditions.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,17 @@
 from chia.types.coin_record import CoinRecord
 from chia.types.coin_spend import CoinSpend
 from chia.types.generator_types import BlockGenerator
 from chia.types.spend_bundle_conditions import SpendBundleConditions
 from chia.util.errors import Err
 from chia.util.ints import uint16, uint32, uint64
 from chia.wallet.puzzles.load_clvm import load_serialized_clvm_maybe_recompile
-from chia.wallet.puzzles.rom_bootstrap_generator import get_generator
-
-GENERATOR_MOD = get_generator()
 
 DESERIALIZE_MOD = load_serialized_clvm_maybe_recompile(
-    "chialisp_deserialisation.clvm", package_or_requirement="chia.wallet.puzzles"
+    "chialisp_deserialisation.clsp", package_or_requirement="chia.wallet.puzzles"
 )
 
 log = logging.getLogger(__name__)
 
 
 def get_name_puzzle_conditions(
     generator: BlockGenerator,
```

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/mempool_manager.py` & `chia-blockchain-1.8.0rc1/chia/full_node/mempool_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/pending_tx_cache.py` & `chia-blockchain-1.8.0rc1/chia/full_node/pending_tx_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/subscriptions.py` & `chia-blockchain-1.8.0rc1/chia/full_node/subscriptions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/sync_store.py` & `chia-blockchain-1.8.0rc1/chia/full_node/sync_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/tx_processing_queue.py` & `chia-blockchain-1.8.0rc1/chia/full_node/tx_processing_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/full_node/weight_proof.py` & `chia-blockchain-1.8.0rc1/chia/full_node/weight_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/harvester/harvester.py` & `chia-blockchain-1.8.0rc1/chia/harvester/harvester.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/harvester/harvester_api.py` & `chia-blockchain-1.8.0rc1/chia/harvester/harvester_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/introducer/introducer.py` & `chia-blockchain-1.8.0rc1/chia/introducer/introducer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/introducer/introducer_api.py` & `chia-blockchain-1.8.0rc1/chia/introducer/introducer_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plot_sync/delta.py` & `chia-blockchain-1.8.0rc1/chia/plot_sync/delta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plot_sync/exceptions.py` & `chia-blockchain-1.8.0rc1/chia/plot_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plot_sync/receiver.py` & `chia-blockchain-1.8.0rc1/chia/plot_sync/receiver.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plot_sync/sender.py` & `chia-blockchain-1.8.0rc1/chia/plot_sync/sender.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plot_sync/util.py` & `chia-blockchain-1.8.0rc1/chia/plot_sync/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotters/bladebit.py` & `chia-blockchain-1.8.0rc1/chia/plotters/bladebit.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotters/chiapos.py` & `chia-blockchain-1.8.0rc1/chia/plotters/chiapos.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotters/madmax.py` & `chia-blockchain-1.8.0rc1/chia/plotters/madmax.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotters/plotters.py` & `chia-blockchain-1.8.0rc1/chia/plotters/plotters.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotters/plotters_util.py` & `chia-blockchain-1.8.0rc1/chia/plotters/plotters_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotting/cache.py` & `chia-blockchain-1.8.0rc1/chia/plotting/cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotting/check_plots.py` & `chia-blockchain-1.8.0rc1/chia/plotting/check_plots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotting/create_plots.py` & `chia-blockchain-1.8.0rc1/chia/plotting/create_plots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotting/manager.py` & `chia-blockchain-1.8.0rc1/chia/plotting/manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/plotting/util.py` & `chia-blockchain-1.8.0rc1/chia/plotting/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/pools/pool_config.py` & `chia-blockchain-1.8.0rc1/chia/pools/pool_config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/pools/pool_puzzles.py` & `chia-blockchain-1.8.0rc1/chia/pools/pool_puzzles.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 from chia.types.coin_spend import CoinSpend, compute_additions
 from chia.util.ints import uint32, uint64
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.puzzles.singleton_top_layer import puzzle_for_singleton
 
 log = logging.getLogger(__name__)
 # "Full" is the outer singleton, with the inner puzzle filled in
-SINGLETON_MOD = load_clvm_maybe_recompile("singleton_top_layer.clvm")
-POOL_WAITING_ROOM_MOD = load_clvm_maybe_recompile("pool_waitingroom_innerpuz.clvm")
-POOL_MEMBER_MOD = load_clvm_maybe_recompile("pool_member_innerpuz.clvm")
-P2_SINGLETON_MOD = load_clvm_maybe_recompile("p2_singleton_or_delayed_puzhash.clvm")
+SINGLETON_MOD = load_clvm_maybe_recompile("singleton_top_layer.clsp")
+POOL_WAITING_ROOM_MOD = load_clvm_maybe_recompile("pool_waitingroom_innerpuz.clsp")
+POOL_MEMBER_MOD = load_clvm_maybe_recompile("pool_member_innerpuz.clsp")
+P2_SINGLETON_MOD = load_clvm_maybe_recompile("p2_singleton_or_delayed_puzhash.clsp")
 POOL_OUTER_MOD = SINGLETON_MOD
 
 POOL_MEMBER_HASH = POOL_MEMBER_MOD.get_tree_hash()
 POOL_WAITING_ROOM_HASH = POOL_WAITING_ROOM_MOD.get_tree_hash()
 P2_SINGLETON_HASH = P2_SINGLETON_MOD.get_tree_hash()
 POOL_OUTER_MOD_HASH = POOL_OUTER_MOD.get_tree_hash()
 SINGLETON_LAUNCHER_HASH = SINGLETON_LAUNCHER.get_tree_hash()
```

### Comparing `chia-blockchain-1.8.0b6/chia/pools/pool_wallet.py` & `chia-blockchain-1.8.0rc1/chia/pools/pool_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/pools/pool_wallet_info.py` & `chia-blockchain-1.8.0rc1/chia/pools/pool_wallet_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/farmer_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/farmer_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/full_node_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/full_node_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/harvester_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/harvester_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/introducer_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/introducer_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/pool_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/pool_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/protocol_message_types.py` & `chia-blockchain-1.8.0rc1/chia/protocols/protocol_message_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/protocol_state_machine.py` & `chia-blockchain-1.8.0rc1/chia/protocols/protocol_state_machine.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/shared_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/shared_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/timelord_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/timelord_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/protocols/wallet_protocol.py` & `chia-blockchain-1.8.0rc1/chia/protocols/wallet_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/pyinstaller.spec` & `chia-blockchain-1.8.0rc1/chia/pyinstaller.spec`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/crawler_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/rpc/crawler_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/rpc/data_layer_rpc_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
             "/get_root_history": self.get_root_history,
             "/add_missing_files": self.add_missing_files,
             "/make_offer": self.make_offer,
             "/take_offer": self.take_offer,
             "/verify_offer": self.verify_offer,
             "/cancel_offer": self.cancel_offer,
             "/get_sync_status": self.get_sync_status,
+            "/check_plugins": self.check_plugins,
         }
 
     async def _state_changed(self, change: str, change_data: Optional[Dict[str, Any]]) -> List[WsRpcMessage]:
         return []
 
     async def create_data_store(self, request: Dict[str, Any]) -> EndpointResult:
         if self.service is None:
@@ -424,7 +425,14 @@
             "sync_status": {
                 "root_hash": sync_status.root_hash.hex(),
                 "generation": sync_status.generation,
                 "target_root_hash": sync_status.target_root_hash.hex(),
                 "target_generation": sync_status.target_generation,
             }
         }
+
+    async def check_plugins(self, request: Dict[str, Any]) -> EndpointResult:
+        if self.service is None:
+            raise Exception("Data layer not created")
+        plugin_status = await self.service.check_plugins()
+
+        return plugin_status.marshal()
```

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_client.py` & `chia-blockchain-1.8.0rc1/chia/rpc/data_layer_rpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,7 +112,11 @@
     async def get_owned_stores(self) -> Dict[str, Any]:
         response = await self.fetch("get_owned_stores", {})
         return response
 
     async def get_sync_status(self, store_id: bytes32) -> Dict[str, Any]:
         response = await self.fetch("get_sync_status", {"id": store_id.hex()})
         return response
+
+    async def check_plugins(self) -> Dict[str, Any]:
+        response = await self.fetch("check_plugins", {})
+        return response
```

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_util.py` & `chia-blockchain-1.8.0rc1/chia/rpc/data_layer_rpc_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/rpc/farmer_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_client.py` & `chia-blockchain-1.8.0rc1/chia/rpc/farmer_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/rpc/full_node_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_client.py` & `chia-blockchain-1.8.0rc1/chia/rpc/full_node_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/rpc/harvester_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_client.py` & `chia-blockchain-1.8.0rc1/chia/rpc/harvester_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/rpc_client.py` & `chia-blockchain-1.8.0rc1/chia/rpc/rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/rpc_server.py` & `chia-blockchain-1.8.0rc1/chia/rpc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/timelord_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/rpc/timelord_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/util.py` & `chia-blockchain-1.8.0rc1/chia/rpc/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/rpc/wallet_rpc_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 from chia.wallet.trading.offer import Offer
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 from chia.wallet.util.address_type import AddressType, is_valid_address
 from chia.wallet.util.compute_hints import compute_coin_hints
 from chia.wallet.util.compute_memos import compute_memos
 from chia.wallet.util.transaction_type import TransactionType
+from chia.wallet.util.wallet_sync_utils import fetch_coin_spend_for_coin_state
 from chia.wallet.util.wallet_types import AmountWithPuzzlehash, WalletType
 from chia.wallet.wallet import CHIP_0002_SIGN_MESSAGE_PREFIX, Wallet
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_info import WalletInfo
 from chia.wallet.wallet_node import WalletNode
 from chia.wallet.wallet_protocol import WalletProtocol
 
@@ -292,17 +293,15 @@
         # Get parent coin
         parent_coin_state_list: List[CoinState] = await self.service.wallet_state_manager.wallet_node.get_coin_state(
             [coin_state.coin.parent_coin_info], peer=peer
         )
         if parent_coin_state_list is None or len(parent_coin_state_list) < 1:
             raise ValueError(f"Parent coin record 0x{coin_state.coin.parent_coin_info.hex()} not found")
         parent_coin_state: CoinState = parent_coin_state_list[0]
-        coin_spend: CoinSpend = await self.service.wallet_state_manager.wallet_node.fetch_puzzle_solution(
-            parent_coin_state.spent_height, parent_coin_state.coin, peer
-        )
+        coin_spend = await fetch_coin_spend_for_coin_state(parent_coin_state, peer)
         return coin_spend, coin_state
 
     ##########################################################################################
     # Key management
     ##########################################################################################
 
     async def log_in(self, request) -> EndpointResult:
@@ -817,17 +816,15 @@
                 # Fetch incoming tx coin spend
                 peer = self.service.get_full_node_peer()
                 assert len(tr.additions) == 1
                 coin_state_list: List[CoinState] = await self.service.wallet_state_manager.wallet_node.get_coin_state(
                     [tr.additions[0].parent_coin_info], peer=peer
                 )
                 assert len(coin_state_list) == 1
-                coin_spend: CoinSpend = await self.service.wallet_state_manager.wallet_node.fetch_puzzle_solution(
-                    coin_state_list[0].spent_height, coin_state_list[0].coin, peer
-                )
+                coin_spend = await fetch_coin_spend_for_coin_state(coin_state_list[0], peer)
                 tr = dataclasses.replace(tr, spend_bundle=SpendBundle([coin_spend], G2Element()))
             else:
                 raise ValueError(f"Transaction 0x{transaction_id.hex()} doesn't have any coin spend.")
         assert tr.spend_bundle is not None
         memos: Dict[bytes32, List[bytes]] = compute_memos(tr.spend_bundle)
         response = {}
         # Convert to hex string
```

### Comparing `chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_client.py` & `chia-blockchain-1.8.0rc1/chia/rpc/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/seeder/crawl_store.py` & `chia-blockchain-1.8.0rc1/chia/seeder/crawl_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/seeder/crawler.py` & `chia-blockchain-1.8.0rc1/chia/seeder/crawler.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/seeder/crawler_api.py` & `chia-blockchain-1.8.0rc1/chia/seeder/crawler_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/seeder/dns_server.py` & `chia-blockchain-1.8.0rc1/chia/seeder/dns_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/seeder/peer_record.py` & `chia-blockchain-1.8.0rc1/chia/seeder/peer_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/seeder/start_crawler.py` & `chia-blockchain-1.8.0rc1/chia/seeder/start_crawler.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/address_manager.py` & `chia-blockchain-1.8.0rc1/chia/server/address_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/address_manager_sqlite_store.py` & `chia-blockchain-1.8.0rc1/chia/server/address_manager_sqlite_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/address_manager_store.py` & `chia-blockchain-1.8.0rc1/chia/server/address_manager_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/chia_policy.py` & `chia-blockchain-1.8.0rc1/chia/server/chia_policy.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/introducer_peers.py` & `chia-blockchain-1.8.0rc1/chia/server/introducer_peers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/node_discovery.py` & `chia-blockchain-1.8.0rc1/chia/server/node_discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from chia.server.address_manager import AddressManager, ExtendedPeerInfo
 from chia.server.address_manager_sqlite_store import create_address_manager_from_db
 from chia.server.address_manager_store import AddressManagerStore
 from chia.server.outbound_message import Message, NodeType, make_msg
 from chia.server.peer_store_resolver import PeerStoreResolver
 from chia.server.server import ChiaServer
 from chia.server.ws_connection import WSChiaConnection
-from chia.types.peer_info import PeerInfo, TimestampedPeerInfo
+from chia.types.peer_info import PeerInfo, TimestampedPeerInfo, UnresolvedPeerInfo
 from chia.util.hash import std_hash
 from chia.util.ints import uint16, uint64
 from chia.util.network import IPAddress, get_host_addr
 
 MAX_PEERS_RECEIVED_PER_REQUEST = 1000
 MAX_TOTAL_PEERS_RECEIVED = 3000
 MAX_CONCURRENT_OUTBOUND_CONNECTIONS = 70
@@ -57,23 +57,17 @@
         self.is_closed = False
         self.target_outbound_count = target_outbound_count
         self.legacy_peer_db_path = peer_store_resolver.legacy_peer_db_path
         self.legacy_peer_db_migrated = False
         self.peers_file_path = peer_store_resolver.peers_file_path
         self.dns_servers = dns_servers
         random.shuffle(dns_servers)  # Don't always start with the same DNS server
+        self.introducer_info: Optional[UnresolvedPeerInfo] = None
         if introducer_info is not None:
-            # get_host_addr is blocking but this only gets called on startup or in the wallet after disconnecting from
-            # all trusted peers.
-            self.introducer_info: Optional[PeerInfo] = PeerInfo(
-                str(get_host_addr(introducer_info["host"], prefer_ipv6=False)),
-                introducer_info["port"],
-            )
-        else:
-            self.introducer_info = None
+            self.introducer_info = UnresolvedPeerInfo(introducer_info["host"], introducer_info["port"])
         self.peer_connect_interval = peer_connect_interval
         self.log = log
         self.relay_queue: Optional[asyncio.Queue[Tuple[TimestampedPeerInfo, int]]] = None
         self.address_manager: Optional[AddressManager] = None
         self.connection_time_pretest: Dict[str, Any] = {}
         self.received_count_from_peers: Dict[str, Any] = {}
         self.lock = asyncio.Lock()
@@ -208,15 +202,17 @@
         if self.introducer_info is None:
             return None
 
         async def on_connect(peer: WSChiaConnection) -> None:
             msg = make_msg(ProtocolMessageTypes.request_peers_introducer, RequestPeersIntroducer())
             await peer.send_message(msg)
 
-        await self.server.start_client(self.introducer_info, on_connect)
+        await self.server.start_client(
+            PeerInfo(get_host_addr(self.introducer_info.host, prefer_ipv6=False), self.introducer_info.port), on_connect
+        )
 
     async def _query_dns(self, dns_address: str) -> None:
         try:
             if self.default_port is None:
                 self.log.error(
                     "Network id not supported in NETWORK_ID_DEFAULT_PORTS neither in config. Skipping DNS query."
                 )
```

### Comparing `chia-blockchain-1.8.0b6/chia/server/outbound_message.py` & `chia-blockchain-1.8.0rc1/chia/server/outbound_message.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/peer_store_resolver.py` & `chia-blockchain-1.8.0rc1/chia/server/peer_store_resolver.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/rate_limit_numbers.py` & `chia-blockchain-1.8.0rc1/chia/server/rate_limit_numbers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/rate_limits.py` & `chia-blockchain-1.8.0rc1/chia/server/rate_limits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/server.py` & `chia-blockchain-1.8.0rc1/chia/server/server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/ssl_context.py` & `chia-blockchain-1.8.0rc1/chia/server/ssl_context.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_data_layer.py` & `chia-blockchain-1.8.0rc1/chia/server/start_data_layer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_farmer.py` & `chia-blockchain-1.8.0rc1/chia/server/start_farmer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_full_node.py` & `chia-blockchain-1.8.0rc1/chia/server/start_full_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,23 @@
     )
 
 
 async def async_main(service_config: Dict[str, Any]) -> int:
     # TODO: refactor to avoid the double load
     config = load_config(DEFAULT_ROOT_PATH, "config.yaml")
     config[SERVICE_NAME] = service_config
-    overrides = service_config["network_overrides"]["constants"][service_config["selected_network"]]
+    network_id = service_config["selected_network"]
+    overrides = service_config["network_overrides"]["constants"][network_id]
+    if network_id == "testnet10":
+        # testnet10 is 1031258 blocks behind mainnet
+        testnet10_offset = 1031258
+        if "SOFT_FORK2_HEIGHT" not in overrides:
+            overrides["SOFT_FORK2_HEIGHT"] = 4000000 - testnet10_offset
+        if "SOFT_FORK_HEIGHT" not in overrides:
+            overrides["SOFT_FORK_HEIGHT"] = 3630000 - testnet10_offset
     updated_constants = DEFAULT_CONSTANTS.replace_str_to_bytes(**overrides)
     initialize_service_logging(service_name=SERVICE_NAME, config=config)
     service = create_full_node_service(DEFAULT_ROOT_PATH, config, updated_constants)
     await service.setup_process_global_state()
     await service.run()
 
     return 0
```

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_harvester.py` & `chia-blockchain-1.8.0rc1/chia/server/start_harvester.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_introducer.py` & `chia-blockchain-1.8.0rc1/chia/server/start_introducer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_service.py` & `chia-blockchain-1.8.0rc1/chia/server/start_service.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_timelord.py` & `chia-blockchain-1.8.0rc1/chia/server/start_timelord.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/start_wallet.py` & `chia-blockchain-1.8.0rc1/chia/server/start_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/upnp.py` & `chia-blockchain-1.8.0rc1/chia/server/upnp.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/server/ws_connection.py` & `chia-blockchain-1.8.0rc1/chia/server/ws_connection.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/block_tools.py` & `chia-blockchain-1.8.0rc1/chia/simulator/block_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import random
 import shutil
 import ssl
 import sys
 import tempfile
 import time
-from dataclasses import replace
+from dataclasses import dataclass, replace
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from blspy import AugSchemeMPL, G1Element, G2Element, PrivateKey
 from chia_rs import compute_merkle_set_root
 from chiabip158 import PyBIP158
 from clvm.casts import int_from_bytes
@@ -41,15 +41,14 @@
 from chia.consensus.vdf_info_computation import get_signage_point_vdf_info
 from chia.daemon.keychain_proxy import KeychainProxy, connect_to_keychain_and_validate, wrap_local_keychain
 from chia.full_node.bundle_tools import (
     best_solution_generator_from_template,
     detect_potential_template_generator,
     simple_solution_generator,
 )
-from chia.full_node.generator import setup_generator_args
 from chia.full_node.signage_point import SignagePoint
 from chia.plotters.chiapos import Params
 from chia.plotting.create_plots import PlotKeys, create_plots
 from chia.plotting.manager import PlotManager
 from chia.plotting.util import (
     PlotRefreshEvents,
     PlotRefreshResult,
@@ -117,17 +116,15 @@
 from chia.util.vdf_prover import get_vdf_info_and_proof
 from chia.wallet.derive_keys import (
     master_sk_to_farmer_sk,
     master_sk_to_local_sk,
     master_sk_to_pool_sk,
     master_sk_to_wallet_sk,
 )
-from chia.wallet.puzzles.rom_bootstrap_generator import get_generator
-
-GENERATOR_MOD = get_generator()
+from chia.wallet.puzzles.rom_bootstrap_generator import GENERATOR_MOD
 
 test_constants = DEFAULT_CONSTANTS.replace(
     **{
         "MIN_PLOT_SIZE": 18,
         "MIN_BLOCKS_PER_CHALLENGE_BLOCK": 12,
         "DIFFICULTY_STARTING": 2**10,
         "DISCRIMINANT_SIZE_BITS": 16,
@@ -354,45 +351,53 @@
     async def setup_plots(
         self,
         num_og_plots: int = 15,
         num_pool_plots: int = 5,
         num_non_keychain_plots: int = 3,
         plot_size: int = 20,
         bitfield: bool = True,
-    ):
+    ) -> bool:
         self.add_plot_directory(self.plot_dir)
         assert self.created_plots == 0
+        existing_plots: bool = True
         # OG Plots
         for i in range(num_og_plots):
-            await self.new_plot(plot_size=plot_size, bitfield=bitfield)
+            plot = await self.new_plot(plot_size=plot_size, bitfield=bitfield)
+            if plot.new_plot:
+                existing_plots = False
         # Pool Plots
         for i in range(num_pool_plots):
-            await self.new_plot(self.pool_ph, plot_size=plot_size, bitfield=bitfield)
+            plot = await self.new_plot(self.pool_ph, plot_size=plot_size, bitfield=bitfield)
+            if plot.new_plot:
+                existing_plots = False
         # Some plots with keys that are not in the keychain
         for i in range(num_non_keychain_plots):
-            await self.new_plot(
+            plot = await self.new_plot(
                 path=self.plot_dir / "not_in_keychain",
                 plot_keys=PlotKeys(G1Element(), G1Element(), None),
                 exclude_plots=True,
                 plot_size=plot_size,
                 bitfield=bitfield,
             )
+            if plot.new_plot:
+                existing_plots = False
         await self.refresh_plots()
         assert len(self.plot_manager.plots) == len(self.expected_plots)
+        return existing_plots
 
     async def new_plot(
         self,
         pool_contract_puzzle_hash: Optional[bytes32] = None,
         path: Path = None,
         tmp_dir: Path = None,
         plot_keys: Optional[PlotKeys] = None,
         exclude_plots: bool = False,
         plot_size: int = 20,
         bitfield: bool = True,
-    ) -> Optional[bytes32]:
+    ) -> BlockToolsNewPlotResult:
         final_dir = self.plot_dir
         if path is not None:
             final_dir = path
             final_dir.mkdir(parents=True, exist_ok=True)
         if tmp_dir is None:
             tmp_dir = self.temp_dir
         params = Params(
@@ -428,29 +433,31 @@
                 use_datetime=False,
                 test_private_keys=[AugSchemeMPL.key_gen(std_hash(self.created_plots.to_bytes(2, "big")))],
             )
             self.created_plots += 1
 
             plot_id_new: Optional[bytes32] = None
             path_new: Optional[Path] = None
+            new_plot: bool = True
 
             if len(created):
                 assert len(existed) == 0
                 plot_id_new, path_new = list(created.items())[0]
 
             if len(existed):
                 assert len(created) == 0
                 plot_id_new, path_new = list(existed.items())[0]
+                new_plot = False
             assert plot_id_new is not None
             assert path_new is not None
 
             if not exclude_plots:
                 self.expected_plots[plot_id_new] = path_new
 
-            return plot_id_new
+            return BlockToolsNewPlotResult(plot_id_new, new_plot)
 
         except KeyboardInterrupt:
             shutil.rmtree(self.temp_dir, ignore_errors=True)
             sys.exit(1)
 
     async def refresh_plots(self) -> None:
         self.plot_manager.refresh_parameter = replace(
@@ -1714,16 +1721,16 @@
     )
 
     return full_block, block_record, block_time_residual
 
 
 def compute_cost_test(generator: BlockGenerator, cost_per_byte: int) -> Tuple[Optional[uint16], uint64]:
     try:
-        block_program, block_program_args = setup_generator_args(generator)
-        clvm_cost, result = GENERATOR_MOD.run_mempool_with_cost(INFINITE_COST, block_program, block_program_args)
+        block_program_args = Program.to([[bytes(g) for g in generator.generator_refs]])
+        clvm_cost, result = GENERATOR_MOD.run_mempool_with_cost(INFINITE_COST, generator.program, block_program_args)
         size_cost = len(bytes(generator.program)) * cost_per_byte
         condition_cost = 0
 
         for res in result.first().as_iter():
             res = res.rest()  # skip parent coind id
             res = res.rest()  # skip puzzle hash
             res = res.rest()  # skip amount
@@ -2117,14 +2124,20 @@
         foliage_transaction_block,
         transactions_info,
         block_generator.program if block_generator else None,
         block_generator.block_height_list if block_generator else [],
     )
 
 
+@dataclass
+class BlockToolsNewPlotResult:
+    plot_id: bytes32
+    new_plot: bool
+
+
 # Remove these counters when `create_block_tools` and `create_block_tools_async` are removed
 create_block_tools_async_count = 0
 create_block_tools_count = 0
 
 # Note: tests that still use `create_block_tools` and `create_block_tools_async` should probably be
 # moved to the bt fixture in conftest.py. Take special care to find out if the users of these functions
 # need different BlockTools instances
```

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/full_node_simulator.py` & `chia-blockchain-1.8.0rc1/chia/simulator/full_node_simulator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/keyring.py` & `chia-blockchain-1.8.0rc1/chia/simulator/keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/setup_nodes.py` & `chia-blockchain-1.8.0rc1/chia/simulator/setup_nodes.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/setup_services.py` & `chia-blockchain-1.8.0rc1/chia/simulator/setup_services.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/simulator_constants.py` & `chia-blockchain-1.8.0rc1/chia/simulator/simulator_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_api.py` & `chia-blockchain-1.8.0rc1/chia/simulator/simulator_full_node_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_client.py` & `chia-blockchain-1.8.0rc1/chia/simulator/simulator_full_node_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/simulator_protocol.py` & `chia-blockchain-1.8.0rc1/chia/simulator/simulator_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/simulator_test_tools.py` & `chia-blockchain-1.8.0rc1/chia/simulator/simulator_test_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/socket.py` & `chia-blockchain-1.8.0rc1/chia/simulator/socket.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_1.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_1.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_10.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_10.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_2.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_2.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_3.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_3.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_4.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_4.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_5.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_5.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_6.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_6.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_7.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_7.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_8.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_8.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_9.py` & `chia-blockchain-1.8.0rc1/chia/simulator/ssl_certs_9.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/start_simulator.py` & `chia-blockchain-1.8.0rc1/chia/simulator/start_simulator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/time_out_assert.py` & `chia-blockchain-1.8.0rc1/chia/simulator/time_out_assert.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/simulator/wallet_tools.py` & `chia-blockchain-1.8.0rc1/chia/simulator/wallet_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/ssl/chia_ca.crt` & `chia-blockchain-1.8.0rc1/chia/ssl/chia_ca.crt`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/ssl/chia_ca.key` & `chia-blockchain-1.8.0rc1/chia/ssl/chia_ca.key`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/ssl/create_ssl.py` & `chia-blockchain-1.8.0rc1/chia/ssl/create_ssl.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/ssl/dst_root_ca.pem` & `chia-blockchain-1.8.0rc1/chia/ssl/dst_root_ca.pem`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/timelord/iters_from_block.py` & `chia-blockchain-1.8.0rc1/chia/timelord/iters_from_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/timelord/timelord.py` & `chia-blockchain-1.8.0rc1/chia/timelord/timelord.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/timelord/timelord_api.py` & `chia-blockchain-1.8.0rc1/chia/timelord/timelord_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/timelord/timelord_launcher.py` & `chia-blockchain-1.8.0rc1/chia/timelord/timelord_launcher.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/timelord/timelord_state.py` & `chia-blockchain-1.8.0rc1/chia/timelord/timelord_state.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/announcement.py` & `chia-blockchain-1.8.0rc1/chia/types/announcement.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/block_protocol.py` & `chia-blockchain-1.8.0rc1/chia/types/block_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/classgroup.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/classgroup.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/coin.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/coin.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/foliage.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/foliage.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/program.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/program.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/proof_of_space.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/proof_of_space.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/reward_chain_block.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/reward_chain_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/serialized_program.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/serialized_program.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/slots.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/slots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/sub_epoch_summary.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/sub_epoch_summary.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/tree_hash.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/tree_hash.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/blockchain_format/vdf.py` & `chia-blockchain-1.8.0rc1/chia/types/blockchain_format/vdf.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/coin_record.py` & `chia-blockchain-1.8.0rc1/chia/types/coin_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/coin_spend.py` & `chia-blockchain-1.8.0rc1/chia/types/coin_spend.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/condition_opcodes.py` & `chia-blockchain-1.8.0rc1/chia/types/condition_opcodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import enum
 from typing import Any
 
 
-# See chia/wallet/puzzles/condition_codes.clvm
+# See chia/wallet/puzzles/condition_codes.clib
 class ConditionOpcode(bytes, enum.Enum):
     # AGG_SIG is ascii "1"
 
     # the conditions below require bls12-381 signatures
 
     AGG_SIG_UNSAFE = bytes([49])
     AGG_SIG_ME = bytes([50])
```

### Comparing `chia-blockchain-1.8.0b6/chia/types/end_of_slot_bundle.py` & `chia-blockchain-1.8.0rc1/chia/types/end_of_slot_bundle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/fee_rate.py` & `chia-blockchain-1.8.0rc1/chia/types/fee_rate.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/full_block.py` & `chia-blockchain-1.8.0rc1/chia/types/full_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/generator_types.py` & `chia-blockchain-1.8.0rc1/chia/types/generator_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/header_block.py` & `chia-blockchain-1.8.0rc1/chia/types/header_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/mempool_item.py` & `chia-blockchain-1.8.0rc1/chia/types/mempool_item.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/mempool_submission_status.py` & `chia-blockchain-1.8.0rc1/chia/types/mempool_submission_status.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/peer_info.py` & `chia-blockchain-1.8.0rc1/chia/types/peer_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/signing_mode.py` & `chia-blockchain-1.8.0rc1/chia/types/signing_mode.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/spend_bundle.py` & `chia-blockchain-1.8.0rc1/chia/types/spend_bundle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/transaction_queue_entry.py` & `chia-blockchain-1.8.0rc1/chia/types/transaction_queue_entry.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/unfinished_block.py` & `chia-blockchain-1.8.0rc1/chia/types/unfinished_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/unfinished_header_block.py` & `chia-blockchain-1.8.0rc1/chia/types/unfinished_header_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/types/weight_proof.py` & `chia-blockchain-1.8.0rc1/chia/types/weight_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/api_decorators.py` & `chia-blockchain-1.8.0rc1/chia/util/api_decorators.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/bech32m.py` & `chia-blockchain-1.8.0rc1/chia/util/bech32m.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/beta_metrics.py` & `chia-blockchain-1.8.0rc1/chia/util/beta_metrics.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/block_cache.py` & `chia-blockchain-1.8.0rc1/chia/util/block_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/byte_types.py` & `chia-blockchain-1.8.0rc1/chia/util/byte_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/cached_bls.py` & `chia-blockchain-1.8.0rc1/chia/util/cached_bls.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/check_fork_next_block.py` & `chia-blockchain-1.8.0rc1/chia/util/check_fork_next_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/chia_logging.py` & `chia-blockchain-1.8.0rc1/chia/util/chia_logging.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/condition_tools.py` & `chia-blockchain-1.8.0rc1/chia/util/condition_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/config.py` & `chia-blockchain-1.8.0rc1/chia/util/config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/create_alert_file.py` & `chia-blockchain-1.8.0rc1/chia/util/create_alert_file.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/db_synchronous.py` & `chia-blockchain-1.8.0rc1/chia/util/db_synchronous.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/db_version.py` & `chia-blockchain-1.8.0rc1/chia/util/db_version.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/db_wrapper.py` & `chia-blockchain-1.8.0rc1/chia/util/db_wrapper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/dump_keyring.py` & `chia-blockchain-1.8.0rc1/chia/util/dump_keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/english.txt` & `chia-blockchain-1.8.0rc1/chia/util/english.txt`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/errors.py` & `chia-blockchain-1.8.0rc1/chia/util/errors.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/file_keyring.py` & `chia-blockchain-1.8.0rc1/chia/util/file_keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/files.py` & `chia-blockchain-1.8.0rc1/chia/util/files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/full_block_utils.py` & `chia-blockchain-1.8.0rc1/chia/util/full_block_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/generator_tools.py` & `chia-blockchain-1.8.0rc1/chia/util/generator_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/initial-config.yaml` & `chia-blockchain-1.8.0rc1/chia/util/initial-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
       DIFFICULTY_STARTING: 30
       EPOCH_BLOCKS: 768
       GENESIS_CHALLENGE: ae83525ba8d1dd3f09b277de18ca3e43fc0af20d20c4b3e92ef2a48bd291ccb2
       GENESIS_PRE_FARM_FARMER_PUZZLE_HASH: 3d8765d3a597ec1d99663f6c9816d915b9f68613ac94009884c4addaefcce6af
       GENESIS_PRE_FARM_POOL_PUZZLE_HASH: d23da14695a188ae5708dd152263c4db883eb27edeb936178d4d988b8f3ce5fc
       MEMPOOL_BLOCK_BUFFER: 10
       MIN_PLOT_SIZE: 18
+      SOFT_FORK_HEIGHT: 2598742
+      SOFT_FORK2_HEIGHT: 2968742
   config:
     mainnet:
       address_prefix: "xch"
       default_full_node_port: 8444
     testnet0:
       address_prefix: "txch"
       default_full_node_port: 58444
```

### Comparing `chia-blockchain-1.8.0b6/chia/util/inline_executor.py` & `chia-blockchain-1.8.0rc1/chia/util/inline_executor.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/ints.py` & `chia-blockchain-1.8.0rc1/chia/util/ints.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/json_util.py` & `chia-blockchain-1.8.0rc1/chia/util/json_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/keychain.py` & `chia-blockchain-1.8.0rc1/chia/util/keychain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/keyring_wrapper.py` & `chia-blockchain-1.8.0rc1/chia/util/keyring_wrapper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/limited_semaphore.py` & `chia-blockchain-1.8.0rc1/chia/util/limited_semaphore.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/lock.py` & `chia-blockchain-1.8.0rc1/chia/util/lock.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/logging.py` & `chia-blockchain-1.8.0rc1/chia/util/logging.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/lru_cache.py` & `chia-blockchain-1.8.0rc1/chia/util/lru_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/merkle_set.py` & `chia-blockchain-1.8.0rc1/chia/util/merkle_set.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/misc.py` & `chia-blockchain-1.8.0rc1/chia/util/misc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/network.py` & `chia-blockchain-1.8.0rc1/chia/util/network.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/paginator.py` & `chia-blockchain-1.8.0rc1/chia/util/paginator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/partial_func.py` & `chia-blockchain-1.8.0rc1/chia/util/partial_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/path.py` & `chia-blockchain-1.8.0rc1/chia/util/path.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/pprint.py` & `chia-blockchain-1.8.0rc1/chia/util/pprint.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/prev_transaction_block.py` & `chia-blockchain-1.8.0rc1/chia/util/prev_transaction_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/profiler.py` & `chia-blockchain-1.8.0rc1/chia/util/profiler.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/service_groups.py` & `chia-blockchain-1.8.0rc1/chia/util/service_groups.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/significant_bits.py` & `chia-blockchain-1.8.0rc1/chia/util/significant_bits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/ssl_check.py` & `chia-blockchain-1.8.0rc1/chia/util/ssl_check.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/streamable.py` & `chia-blockchain-1.8.0rc1/chia/util/streamable.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/struct_stream.py` & `chia-blockchain-1.8.0rc1/chia/util/struct_stream.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/task_timing.py` & `chia-blockchain-1.8.0rc1/chia/util/task_timing.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/validate_alert.py` & `chia-blockchain-1.8.0rc1/chia/util/validate_alert.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/vdf_prover.py` & `chia-blockchain-1.8.0rc1/chia/util/vdf_prover.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/util/ws_message.py` & `chia-blockchain-1.8.0rc1/chia/util/ws_message.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/block_record.py` & `chia-blockchain-1.8.0rc1/chia/wallet/block_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_constants.py` & `chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_info.py` & `chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_outer_puzzle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_utils.py` & `chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_wallet.py` & `chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/cat_wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 )
 from chia.wallet.puzzles.tails import ALL_LIMITATIONS_PROGRAMS
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 from chia.wallet.util.compute_memos import compute_memos
 from chia.wallet.util.curry_and_treehash import calculate_hash_of_quoted_mod_hash, curry_and_treehash
 from chia.wallet.util.transaction_type import TransactionType
+from chia.wallet.util.wallet_sync_utils import fetch_coin_spend_for_coin_state
 from chia.wallet.util.wallet_types import AmountWithPuzzlehash, WalletType
 from chia.wallet.wallet import Wallet
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_info import WalletInfo
 
 if TYPE_CHECKING:
     from chia.wallet.wallet_state_manager import WalletStateManager
@@ -343,17 +344,15 @@
 
         if lineage is None:
             try:
                 coin_state = await self.wallet_state_manager.wallet_node.get_coin_state(
                     [coin.parent_coin_info], peer=peer
                 )
                 assert coin_state[0].coin.name() == coin.parent_coin_info
-                coin_spend = await self.wallet_state_manager.wallet_node.fetch_puzzle_solution(
-                    coin_state[0].spent_height, coin_state[0].coin, peer
-                )
+                coin_spend = await fetch_coin_spend_for_coin_state(coin_state[0], peer)
                 await self.puzzle_solution_received(coin_spend, parent_coin=coin_state[0].coin)
             except Exception as e:
                 self.log.debug(f"Exception: {e}, traceback: {traceback.format_exc()}")
 
     async def puzzle_solution_received(self, coin_spend: CoinSpend, parent_coin: Coin) -> None:
         coin_name = coin_spend.coin.name()
         puzzle: Program = Program.from_bytes(bytes(coin_spend.puzzle_reveal))
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/lineage_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/cat_wallet/lineage_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/chialisp.py` & `chia-blockchain-1.8.0rc1/chia/wallet/chialisp.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/coin_selection.py` & `chia-blockchain-1.8.0rc1/chia/wallet/coin_selection.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/db_wallet/db_wallet_puzzles.py` & `chia-blockchain-1.8.0rc1/chia/wallet/db_wallet/db_wallet_puzzles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 
 # from chia.types.condition_opcodes import ConditionOpcode
 # from chia.wallet.util.merkle_tree import MerkleTree, TreeType
 
 ACS_MU = Program.to(11)  # returns the third argument a.k.a the full solution
 ACS_MU_PH = ACS_MU.get_tree_hash()
-SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clvm")
-SINGLETON_LAUNCHER = load_clvm_maybe_recompile("singleton_launcher.clvm")
-GRAFTROOT_DL_OFFERS = load_clvm_maybe_recompile("graftroot_dl_offers.clvm")
-P2_PARENT = load_clvm_maybe_recompile("p2_parent.clvm")
+SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clsp")
+SINGLETON_LAUNCHER = load_clvm_maybe_recompile("singleton_launcher.clsp")
+GRAFTROOT_DL_OFFERS = load_clvm_maybe_recompile("graftroot_dl_offers.clsp")
+P2_PARENT = load_clvm_maybe_recompile("p2_parent.clsp")
 
 
 def create_host_fullpuz(innerpuz: Union[Program, bytes32], current_root: bytes32, genesis_id: bytes32) -> Program:
     db_layer = create_host_layer_puzzle(innerpuz, current_root)
     mod_hash = SINGLETON_TOP_LAYER_MOD.get_tree_hash()
     singleton_struct = Program.to((mod_hash, (genesis_id, SINGLETON_LAUNCHER.get_tree_hash())))
     return SINGLETON_TOP_LAYER_MOD.curry(singleton_struct, db_layer)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/derivation_record.py` & `chia-blockchain-1.8.0rc1/chia/wallet/derivation_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/derive_keys.py` & `chia-blockchain-1.8.0rc1/chia/wallet/derive_keys.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_info.py` & `chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/did_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet.py` & `chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/did_wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     create_singleton_puzzle,
     create_singleton_puzzle_hash,
     get_inner_puzzle_from_singleton,
 )
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.util.compute_memos import compute_memos
 from chia.wallet.util.transaction_type import TransactionType
+from chia.wallet.util.wallet_sync_utils import fetch_coin_spend
 from chia.wallet.util.wallet_types import WalletType
 from chia.wallet.wallet import CHIP_0002_SIGN_MESSAGE_PREFIX, Wallet
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_info import WalletInfo
 
 
 class DIDWallet:
@@ -501,15 +502,15 @@
                     bytes(new_pubkey),
                     did_info.sent_recovery_transaction,
                     did_info.metadata,
                 )
 
                 await self.save_info(did_info)
                 assert children_state.created_height
-                parent_spend = await wallet_node.fetch_puzzle_solution(children_state.created_height, parent_coin, peer)
+                parent_spend = await fetch_coin_spend(uint32(children_state.created_height), parent_coin, peer)
                 assert parent_spend is not None
                 parent_innerpuz = get_inner_puzzle_from_singleton(parent_spend.puzzle_reveal.to_program())
                 assert parent_innerpuz is not None
                 parent_info = LineageProof(
                     parent_coin.parent_coin_info,
                     parent_innerpuz.get_tree_hash(),
                     uint64(parent_coin.amount),
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet_puzzles.py` & `chia-blockchain-1.8.0rc1/chia/wallet/did_wallet/did_wallet_puzzles.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     SINGLETON_LAUNCHER_PUZZLE_HASH,
     SINGLETON_TOP_LAYER_MOD,
     SINGLETON_TOP_LAYER_MOD_HASH,
     is_singleton,
 )
 from chia.wallet.util.curry_and_treehash import calculate_hash_of_quoted_mod_hash, curry_and_treehash
 
-DID_INNERPUZ_MOD = load_clvm_maybe_recompile("did_innerpuz.clvm")
+DID_INNERPUZ_MOD = load_clvm_maybe_recompile("did_innerpuz.clsp")
 DID_INNERPUZ_MOD_HASH = DID_INNERPUZ_MOD.get_tree_hash()
-INTERMEDIATE_LAUNCHER_MOD = load_clvm_maybe_recompile("nft_intermediate_launcher.clvm")
+INTERMEDIATE_LAUNCHER_MOD = load_clvm_maybe_recompile("nft_intermediate_launcher.clsp")
 
 
 def create_innerpuz(
     p2_puzzle: Program,
     recovery_list: List[bytes32],
     num_of_backup_ids_needed: uint64,
     launcher_id: bytes32,
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/driver_protocol.py` & `chia-blockchain-1.8.0rc1/chia/wallet/driver_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/key_val_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/key_val_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/lineage_proof.py` & `chia-blockchain-1.8.0rc1/chia/wallet/lineage_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/metadata_outer_puzzle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/metadata_outer_puzzle.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.util.ints import uint64
 from chia.wallet.puzzle_drivers import PuzzleInfo, Solver
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.uncurried_puzzle import UncurriedPuzzle, uncurry_puzzle
 
-NFT_STATE_LAYER_MOD = load_clvm_maybe_recompile("nft_state_layer.clvm")
+NFT_STATE_LAYER_MOD = load_clvm_maybe_recompile("nft_state_layer.clsp")
 NFT_STATE_LAYER_MOD_HASH = NFT_STATE_LAYER_MOD.get_tree_hash()
 
 
 def match_metadata_layer_puzzle(puzzle: UncurriedPuzzle) -> Tuple[bool, List[Program]]:
     if puzzle.mod == NFT_STATE_LAYER_MOD:
         return True, list(puzzle.args.as_iter())
     return False, []
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_info.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/nft_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.util.ints import uint16, uint32, uint64
 from chia.util.streamable import Streamable, streamable
 from chia.wallet.lineage_proof import LineageProof
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 
-LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clvm")
+LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clsp")
 IN_TRANSACTION_STATUS = "IN_TRANSACTION"
 DEFAULT_STATUS = "DEFAULT"
 
 
 @streamable
 @dataclass(frozen=True)
 class NFTInfo(Streamable):
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_puzzles.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/nft_puzzles.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,34 +14,34 @@
 from chia.wallet.nft_wallet.nft_info import NFTCoinInfo, NFTInfo
 from chia.wallet.nft_wallet.uncurry_nft import UncurriedNFT
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import solution_for_conditions
 from chia.wallet.util.address_type import AddressType
 
 log = logging.getLogger(__name__)
-SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clvm")
-LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clvm")
-NFT_STATE_LAYER_MOD = load_clvm_maybe_recompile("nft_state_layer.clvm")
+SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clsp")
+LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clsp")
+NFT_STATE_LAYER_MOD = load_clvm_maybe_recompile("nft_state_layer.clsp")
 LAUNCHER_PUZZLE_HASH = LAUNCHER_PUZZLE.get_tree_hash()
 SINGLETON_MOD_HASH = SINGLETON_TOP_LAYER_MOD.get_tree_hash()
 NFT_STATE_LAYER_MOD_HASH = NFT_STATE_LAYER_MOD.get_tree_hash()
-NFT_METADATA_UPDATER = load_clvm_maybe_recompile("nft_metadata_updater_default.clvm")
-NFT_OWNERSHIP_LAYER = load_clvm_maybe_recompile("nft_ownership_layer.clvm")
+NFT_METADATA_UPDATER = load_clvm_maybe_recompile("nft_metadata_updater_default.clsp")
+NFT_OWNERSHIP_LAYER = load_clvm_maybe_recompile("nft_ownership_layer.clsp")
 NFT_OWNERSHIP_LAYER_HASH = NFT_OWNERSHIP_LAYER.get_tree_hash()
 NFT_TRANSFER_PROGRAM_DEFAULT = load_clvm_maybe_recompile(
-    "nft_ownership_transfer_program_one_way_claim_with_royalties.clvm",
+    "nft_ownership_transfer_program_one_way_claim_with_royalties.clsp",
 )
-STANDARD_PUZZLE_MOD = load_clvm_maybe_recompile("p2_delegated_puzzle_or_hidden_puzzle.clvm")
-INTERMEDIATE_LAUNCHER_MOD = load_clvm_maybe_recompile("nft_intermediate_launcher.clvm")
+STANDARD_PUZZLE_MOD = load_clvm_maybe_recompile("p2_delegated_puzzle_or_hidden_puzzle.clsp")
+INTERMEDIATE_LAUNCHER_MOD = load_clvm_maybe_recompile("nft_intermediate_launcher.clsp")
 
 
 def create_nft_layer_puzzle_with_curry_params(
     metadata: Program, metadata_updater_hash: bytes32, inner_puzzle: Program
 ) -> Program:
-    """Curries params into nft_state_layer.clvm
+    """Curries params into nft_state_layer.clsp
 
     Args to curry:
         NFT_STATE_LAYER_MOD_HASH
         METADATA
         METADATA_UPDATER_PUZZLE_HASH
         INNER_PUZZLE"""
     return NFT_STATE_LAYER_MOD.curry(NFT_STATE_LAYER_MOD_HASH, metadata, metadata_updater_hash, inner_puzzle)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_wallet.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/nft_wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     NotarizedPayment,
     Offer,
 )
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 from chia.wallet.util.compute_memos import compute_memos
 from chia.wallet.util.transaction_type import TransactionType
+from chia.wallet.util.wallet_sync_utils import fetch_coin_spend
 from chia.wallet.util.wallet_types import AmountWithPuzzlehash, WalletType
 from chia.wallet.wallet import CHIP_0002_SIGN_MESSAGE_PREFIX, Wallet
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_info import WalletInfo
 from chia.wallet.wallet_nft_store import WalletNftStore
 
 _T_NFTWallet = TypeVar("_T_NFTWallet", bound="NFTWallet")
@@ -166,15 +167,15 @@
         cs: Optional[CoinSpend] = None
         coin_states: Optional[List[CoinState]] = await wallet_node.get_coin_state([coin.parent_coin_info], peer=peer)
         if not coin_states:
             # farm coin
             return
         assert coin_states
         parent_coin = coin_states[0].coin
-        cs = await wallet_node.fetch_puzzle_solution(height, parent_coin, peer)
+        cs = await fetch_coin_spend(height, parent_coin, peer)
         assert cs is not None
         await self.puzzle_solution_received(cs, peer)
 
     async def puzzle_solution_received(self, coin_spend: CoinSpend, peer: WSChiaConnection) -> None:
         self.log.debug("Puzzle solution received to wallet: %s", self.wallet_info)
         coin_name = coin_spend.coin.name()
         puzzle: Program = Program.from_bytes(bytes(coin_spend.puzzle_reveal))
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/ownership_outer_puzzle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/ownership_outer_puzzle.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.wallet.puzzle_drivers import PuzzleInfo, Solver
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.uncurried_puzzle import UncurriedPuzzle, uncurry_puzzle
 
-OWNERSHIP_LAYER_MOD = load_clvm_maybe_recompile("nft_ownership_layer.clvm")
+OWNERSHIP_LAYER_MOD = load_clvm_maybe_recompile("nft_ownership_layer.clsp")
 
 
 def match_ownership_layer_puzzle(puzzle: UncurriedPuzzle) -> Tuple[bool, List[Program]]:
     if puzzle.mod == OWNERSHIP_LAYER_MOD:
         return True, list(puzzle.args.as_iter())
     return False, []
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/singleton_outer_puzzle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/singleton_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/transfer_program_puzzle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/transfer_program_puzzle.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.util.ints import uint16
 from chia.wallet.puzzle_drivers import PuzzleInfo, Solver
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.puzzles.singleton_top_layer_v1_1 import SINGLETON_LAUNCHER_HASH, SINGLETON_MOD_HASH
 from chia.wallet.uncurried_puzzle import UncurriedPuzzle
 
-TRANSFER_PROGRAM_MOD = load_clvm_maybe_recompile("nft_ownership_transfer_program_one_way_claim_with_royalties.clvm")
+TRANSFER_PROGRAM_MOD = load_clvm_maybe_recompile("nft_ownership_transfer_program_one_way_claim_with_royalties.clsp")
 
 
 def match_transfer_program_puzzle(puzzle: UncurriedPuzzle) -> Tuple[bool, List[Program]]:
     if puzzle.mod == TRANSFER_PROGRAM_MOD:
         return True, list(puzzle.args.as_iter())
     return False, []
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/uncurry_nft.py` & `chia-blockchain-1.8.0rc1/chia/wallet/nft_wallet/uncurry_nft.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.util.ints import uint16
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 
 log = logging.getLogger(__name__)
-SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clvm")
-NFT_MOD = load_clvm_maybe_recompile("nft_state_layer.clvm")
-NFT_OWNERSHIP_LAYER = load_clvm_maybe_recompile("nft_ownership_layer.clvm")
+SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clsp")
+NFT_MOD = load_clvm_maybe_recompile("nft_state_layer.clsp")
+NFT_OWNERSHIP_LAYER = load_clvm_maybe_recompile("nft_ownership_layer.clsp")
 
 _T_UncurriedNFT = TypeVar("_T_UncurriedNFT", bound="UncurriedNFT")
 
 
 @dataclass(frozen=True)
 class UncurriedNFT:
     """
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/notification_manager.py` & `chia-blockchain-1.8.0rc1/chia/wallet/notification_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/notification_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/notification_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/outer_puzzles.py` & `chia-blockchain-1.8.0rc1/chia/wallet/outer_puzzles.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/payment.py` & `chia-blockchain-1.8.0rc1/chia/wallet/payment.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzle_drivers.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzle_drivers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/block_program_zero.clsp`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_truths.clib` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/cat_truths.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/cat_v2.clsp`

 * *Files 10% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-; Coins locked with this puzzle are spendable cats.
-;
-; Choose a list of n inputs (n>=1), I_1, ... I_n with amounts A_1, ... A_n.
-;
-; We put them in a ring, so "previous" and "next" have intuitive k-1 and k+1 semantics,
-; wrapping so {n} and 0 are the same, ie. all indices are mod n.
-;
-; Each coin creates 0 or more coins with total output value O_k.
-; Let D_k = the "debt" O_k - A_k contribution of coin I_k, ie. how much debt this input accumulates.
-; Some coins may spend more than they contribute and some may spend less, ie. D_k need
-; not be zero. That's okay. It's enough for the total of all D_k in the ring to be 0.
-;
-; A coin can calculate its own D_k since it can verify A_k (it's hashed into the coin id)
-; and it can sum up `CREATE_COIN` conditions for O_k.
-;
-; Defines a "subtotal of debts" S_k for each coin as follows:
-;
-; S_1 = 0
-; S_k = S_{k-1} + D_{k-1}
-;
-; Here's the main trick that shows the ring sums to 0.
-; You can prove by induction that S_{k+1} = D_1 + D_2 + ... + D_k.
-; But it's a ring, so S_{n+1} is also S_1, which is 0. So D_1 + D_2 + ... + D_k = 0.
-; So the total debts must be 0, ie. no coins are created or destroyed.
-;
-; Each coin's solution includes I_{k-1}, I_k, and I_{k+1} along with proofs that I_{k}, and I_{k+1} are CATs of the same type.
-; Each coin's solution includes S_{k-1}. It calculates D_k = O_k - A_k, and then S_k = S_{k-1} + D_{k-1}
-;
-; Announcements are used to ensure that each S_k follows the pattern is valid.
-; Announcements automatically commit to their own coin id.
-; Coin I_k creates an announcement that further commits to I_{k-1} and S_{k-1}.
-;
-; Coin I_k gets a proof that I_{k+1} is a cat, so it knows it must also create an announcement
-; when spent. It checks that I_{k+1} creates an announcement committing to I_k and S_k.
-;
-; So S_{k+1} is correct iff S_k is correct.
-;
-; Coins also receive proofs that their neighbours are CATs, ensuring the announcements aren't forgeries.
-; Inner puzzles and the CAT layer prepend `CREATE_COIN_ANNOUNCEMENT` with different prefixes to avoid forgeries.
-; Ring announcements use 0xcb, and inner puzzles are given 0xca
-;
-; In summary, I_k generates a coin_announcement Y_k ("Y" for "yell") as follows:
-;
-;  Y_k: hash of I_k (automatically), I_{k-1}, S_k
-;
-; Each coin creates an assert_coin_announcement to ensure that the next coin's announcement is as expected:
-;  Y_{k+1} : hash of I_{k+1}, I_k, S_{k+1}
-;
-; TLDR:
-;  I_k : coins
-;  A_k : amount coin k contributes
-;  O_k : amount coin k spend
-;  D_k : difference/delta that coin k incurs (A - O)
-;  S_k : subtotal of debts D_1 + D_2 ... + D_k
-;  Y_k : announcements created by coin k committing to I_{k-1}, I_k, S_k
-;
-; All conditions go through a "transformer" that looks for CREATE_COIN conditions
-; generated by the inner solution, and wraps the puzzle hash ensuring the output is a cat.
-;
-; Three output conditions are prepended to the list of conditions for each I_k:
-;  (ASSERT_MY_ID I_k) to ensure that the passed in value for I_k is correct
-;  (CREATE_COIN_ANNOUNCEMENT I_{k-1} S_k) to create this coin's announcement
-;  (ASSERT_COIN_ANNOUNCEMENT hashed_announcement(Y_{k+1})) to ensure the next coin really is next and
-;     the relative values of S_k and S_{k+1} are correct
-;
-; This is all we need to do to ensure cats exactly balance in the inputs and outputs.
-;
-; Proof:
-;   Consider n, k, I_k values, O_k values, S_k and A_k as above.
-;   For the (CREATE_COIN_ANNOUNCEMENT Y_{k+1}) (created by the next coin)
-;   and (ASSERT_COIN_ANNOUNCEMENT hashed(Y_{k+1})) to match,
-;   we see that I_k can ensure that is has the correct value for S_{k+1}.
-;
-;   By induction, we see that S_{m+1} = sum(i, 1, m) [O_i - A_i] = sum(i, 1, m) O_i - sum(i, 1, m) A_i
-;   So S_{n+1} = sum(i, 1, n) O_i - sum(i, 1, n) A_i. But S_{n+1} is actually S_1 = 0,
-;   so thus sum(i, 1, n) O_i = sum (i, 1, n) A_i, ie. output total equals input total.
-
-;; GLOSSARY:
-;;  MOD_HASH: this code's sha256 tree hash
-;;  TAIL_PROGRAM_HASH: the program that determines if a coin can mint new cats, burn cats, and check if its lineage is valid if its parent is not a CAT
-;;  INNER_PUZZLE: an independent puzzle protecting the coins. Solutions to this puzzle are expected to generate `AGG_SIG` conditions and possibly `CREATE_COIN` conditions.
-;; ---- items above are curried into the puzzle hash ----
-;;  inner_puzzle_solution: the solution to the inner puzzle
-;;  prev_coin_id: the id for the previous coin
-;;  tail_program_reveal: reveal of TAIL_PROGRAM_HASH required to run the program if desired
-;;  tail_solution: optional solution passed into tail_program
-;;  lineage_proof: optional proof that our coin's parent is a CAT
-;;  this_coin_info: (parent_id puzzle_hash amount)
-;;  next_coin_proof: (parent_id inner_puzzle_hash amount)
-;;  prev_subtotal: the subtotal between prev-coin and this-coin
-;;  extra_delta: an amount that is added to our delta and checked by the TAIL program
-;;
-
-(mod (
-      MOD_HASH                 ;; curried into puzzle
-      TAIL_PROGRAM_HASH        ;; curried into puzzle
-      INNER_PUZZLE             ;; curried into puzzle
-      inner_puzzle_solution    ;; if invalid, INNER_PUZZLE will fail
-      lineage_proof            ;; This is the parent's coin info, used to check if the parent was a CAT. Optional if using tail_program.
-      prev_coin_id             ;; used in this coin's announcement, prev_coin ASSERT_COIN_ANNOUNCEMENT will fail if wrong
-      this_coin_info           ;; verified with ASSERT_MY_COIN_ID
-      next_coin_proof          ;; used to generate ASSERT_COIN_ANNOUNCEMENT
-      prev_subtotal            ;; included in announcement, prev_coin ASSERT_COIN_ANNOUNCEMENT will fail if wrong
-      extra_delta              ;; this is the "legal discrepancy" between your real delta and what you're announcing your delta is
-    )
-
-     ;;;;; start library code
-
-     (include condition_codes.clvm)
-     (include curry-and-treehash.clinc)
-     (include cat_truths.clib)
-     (include utility_macros.clib)
-
-     (defconstant RING_MORPH_BYTE 0xcb)
-
-
-    ; take two lists and merge them into one
-    (defun merge_list (list_a list_b)
-      (if list_a
-        (c (f list_a) (merge_list (r list_a) list_b))
-        list_b
-      )
-    )
-
-    ; cat_mod_struct = (MOD_HASH MOD_HASH_hash GENESIS_COIN_CHECKER GENESIS_COIN_CHECKER_hash)
-
-    (defun-inline mod_hash_from_cat_mod_struct (cat_mod_struct) (f cat_mod_struct))
-    (defun-inline mod_hash_hash_from_cat_mod_struct (cat_mod_struct) (f (r cat_mod_struct)))
-    (defun-inline tail_program_hash_from_cat_mod_struct (cat_mod_struct) (f (r (r cat_mod_struct))))
-
-     ;;;;; end library code
-
-     ;; return the puzzle hash for a cat with the given `GENESIS_COIN_CHECKER_hash` & `INNER_PUZZLE`
-     (defun-inline cat_puzzle_hash (cat_mod_struct inner_puzzle_hash)
-       (puzzle-hash-of-curried-function (mod_hash_from_cat_mod_struct cat_mod_struct)
-                                        inner_puzzle_hash
-                                        (sha256 ONE (tail_program_hash_from_cat_mod_struct cat_mod_struct))
-                                        (mod_hash_hash_from_cat_mod_struct cat_mod_struct)
-       )
-     )
-
-     ;; assert `CREATE_COIN_ANNOUNCEMENT` doesn't contain the RING_MORPH_BYTE bytes so it cannot be used to cheat the coin ring
-
-     (defun-inline morph_condition (condition cat_mod_struct)
-       (if (= (f condition) CREATE_COIN)
-         (c CREATE_COIN
-               (c (cat_puzzle_hash cat_mod_struct (f (r condition)))
-                    (r (r condition)))
-         )
-         (if (= (f condition) CREATE_COIN_ANNOUNCEMENT)
-           (assert (not (and
-                     (= 33 (strlen (f (r condition))))
-                     (= (substr (f (r condition)) 0 ONE) RING_MORPH_BYTE)  ; lazy eval
-                   ))
-             ; then
-             condition
-           )
-           condition
-         )
-       )
-     )
-
-     ;; given a coin's parent, inner_puzzle and amount, and the cat_mod_struct, calculate the id of the coin
-     (defun-inline coin_id_for_proof (coin cat_mod_struct)
-       (calculate_coin_id (f coin) (cat_puzzle_hash cat_mod_struct (f (r coin))) (f (r (r coin))))
-     )
-
-     ;; utility to fetch coin amount from coin
-     (defun-inline input_amount_for_coin (coin)
-       (f (r (r coin)))
-     )
-
-     ;; calculate the hash of an announcement
-     ;; we add 0xcb so ring announcements exist in a different namespace to announcements from inner_puzzles
-     (defun-inline calculate_annoucement_id (this_coin_id this_subtotal next_coin_id cat_mod_struct)
-       (sha256 next_coin_id RING_MORPH_BYTE (sha256tree (list this_coin_id this_subtotal)))
-     )
-
-     ;; create the `ASSERT_COIN_ANNOUNCEMENT` condition that ensures the next coin's announcement is correct
-     (defun-inline create_assert_next_announcement_condition (this_coin_id this_subtotal next_coin_id cat_mod_struct)
-       (list ASSERT_COIN_ANNOUNCEMENT
-             (calculate_annoucement_id this_coin_id
-                                            this_subtotal
-                                            next_coin_id
-                                            cat_mod_struct
-             )
-       )
-     )
-
-     ;; here we commit to I_{k-1} and S_k
-     ;; we add 0xcb so ring announcements exist in a different namespace to announcements from inner_puzzles
-     (defun-inline create_announcement_condition (prev_coin_id prev_subtotal)
-       (list CREATE_COIN_ANNOUNCEMENT
-             (concat RING_MORPH_BYTE (sha256tree (list prev_coin_id prev_subtotal)))
-       )
-      )
-
-     ;;;;;;;;;;;;;;;;;;;;;;;;;;;
-
-     ;; this function takes a condition and returns an integer indicating
-     ;; the value of all output coins created with CREATE_COIN. If it's not
-     ;; a CREATE_COIN condition, it returns 0.
-
-     (defun-inline output_value_for_condition (condition)
-       (if (= (f condition) CREATE_COIN)
-         (f (r (r condition)))
-         0
-       )
-     )
-
-     ;; add two conditions to the list of morphed conditions:
-     ;; CREATE_COIN_ANNOUNCEMENT for my announcement
-     ;; ASSERT_COIN_ANNOUNCEMENT for the next coin's announcement
-     (defun-inline generate_final_output_conditions
-       (
-         prev_subtotal
-         this_subtotal
-         morphed_conditions
-         prev_coin_id
-         this_coin_id
-         next_coin_id
-         cat_mod_struct
-       )
-         (c (create_announcement_condition prev_coin_id prev_subtotal)
-           (c (create_assert_next_announcement_condition this_coin_id this_subtotal next_coin_id cat_mod_struct)
-             morphed_conditions)
-         )
-      )
-
-
-      ;; This next section of code loops through all of the conditions to do three things:
-      ;;   1) Look for a "magic" value of -113 and, if one exists, filter it, and take note of the tail reveal and solution
-      ;;   2) Morph any CREATE_COIN or CREATE_COIN_ANNOUNCEMENT conditions
-      ;;   3) Sum the total output amount of all of the CREATE_COINs that are output by the inner puzzle
-      ;;
-      ;; After everything return a struct in the format (morphed_conditions . (output_sum . tail_reveal_and_solution))
-      ;; If multiple magic conditions are specified, the later one will take precedence
-
-      (defun-inline condition_tail_reveal (condition) (f (r (r (r condition)))))
-      (defun-inline condition_tail_solution (condition) (f (r (r (r (r condition))))))
-
-      (defun cons_onto_first_and_add_to_second (morphed_condition output_value struct)
-        (c (c morphed_condition (f struct)) (c (+ output_value (f (r struct))) (r (r struct))))
-      )
-
-      (defun find_and_strip_tail_info (inner_conditions cat_mod_struct tail_reveal_and_solution)
-        (if inner_conditions
-            (if (= (output_value_for_condition (f inner_conditions)) -113)  ; Checks this is a CREATE_COIN of value -113
-                (find_and_strip_tail_info
-                  (r inner_conditions)
-                  cat_mod_struct
-                  (c (condition_tail_reveal (f inner_conditions)) (condition_tail_solution (f inner_conditions)))
-                )
-                (cons_onto_first_and_add_to_second
-                  (morph_condition (f inner_conditions) cat_mod_struct)
-                  (output_value_for_condition (f inner_conditions))
-                  (find_and_strip_tail_info
-                    (r inner_conditions)
-                    cat_mod_struct
-                    tail_reveal_and_solution
-                  )
-                )
-            )
-            (c () (c 0 tail_reveal_and_solution))
-        )
-      )
-
-     ;;;;;;;;;;;;;;;;;;;;;;;;;;; lineage checking
-
-     ;; return true iff parent of `this_coin_info` is provably a cat
-     ;; A 'lineage proof' consists of (parent_parent_id parent_INNER_puzzle_hash parent_amount)
-     ;; We use this information to construct a coin who's puzzle has been wrapped in this MOD and verify that,
-     ;; once wrapped, it matches our parent coin's ID.
-     (defun-inline is_parent_cat (
-       cat_mod_struct
-       parent_id
-       lineage_proof
-     )
-       (= parent_id
-          (calculate_coin_id (f lineage_proof)
-                  (cat_puzzle_hash cat_mod_struct (f (r lineage_proof)))
-                  (f (r (r lineage_proof)))
-          )
-       )
-     )
-
-    (defun check_lineage_or_run_tail_program
-      (
-        this_coin_info
-        tail_reveal_and_solution
-        parent_is_cat  ; flag which says whether or not the parent CAT check ran and passed
-        lineage_proof
-        Truths
-        extra_delta
-        inner_conditions
-      )
-      (if tail_reveal_and_solution
-          (assert (= (sha256tree (f tail_reveal_and_solution)) (cat_tail_program_hash_truth Truths))
-            (merge_list
-              (a  (f tail_reveal_and_solution)
-                  (list
-                    Truths
-                    parent_is_cat
-                    lineage_proof ; Lineage proof is only guaranteed to be true if parent_is_cat
-                    extra_delta
-                    inner_conditions
-                    (r tail_reveal_and_solution)
-                  )
-              )
-              inner_conditions
-            )
-          )
-          (assert parent_is_cat (not extra_delta)
-            inner_conditions
-          )
-      )
-    )
-
-     ;;;;;;;;;;;;;;;;;;;;;;;;;;;
-
-     (defun stager_two (
-         Truths
-         (inner_conditions . (output_sum . tail_reveal_and_solution))
-         lineage_proof
-         prev_coin_id
-         this_coin_info
-         next_coin_id
-         prev_subtotal
-         extra_delta
-      )
-      (check_lineage_or_run_tail_program
-            this_coin_info
-            tail_reveal_and_solution
-            (if lineage_proof (is_parent_cat (cat_struct_truth Truths) (my_parent_cat_truth Truths) lineage_proof) ())
-            lineage_proof
-            Truths
-            extra_delta
-            (generate_final_output_conditions
-              prev_subtotal
-              ; the expression on the next line calculates `this_subtotal` by adding the delta to `prev_subtotal`
-              (+ prev_subtotal (- (input_amount_for_coin this_coin_info) output_sum) extra_delta)
-              inner_conditions
-              prev_coin_id
-              (my_id_cat_truth Truths)
-              next_coin_id
-              (cat_struct_truth Truths)
-            )
-        )
-    )
-
-    ; CAT TRUTHS struct is: ; CAT Truths is: ((Inner puzzle hash . (MOD hash . (MOD hash hash . TAIL hash))) . (my_id . (my_parent_info my_puzhash my_amount)))
-    ; create truths - this_coin_info verified true because we calculated my ID from it!
-    ; lineage proof is verified later by cat parent check or tail_program
-
-    (defun stager (
-        cat_mod_struct
-        inner_conditions
-        lineage_proof
-        inner_puzzle_hash
-        my_id
-        prev_coin_id
-        this_coin_info
-        next_coin_proof
-        prev_subtotal
-        extra_delta
-     )
-      (c (list ASSERT_MY_COIN_ID my_id) (stager_two
-        (cat_truth_data_to_truth_struct
-          inner_puzzle_hash
-          cat_mod_struct
-          my_id
-          this_coin_info
-        )
-        (find_and_strip_tail_info inner_conditions cat_mod_struct ())
-        lineage_proof
-        prev_coin_id
-        this_coin_info
-        (coin_id_for_proof next_coin_proof cat_mod_struct)
-        prev_subtotal
-        extra_delta
-      ))
-    )
-
-    (stager
-        ;; calculate cat_mod_struct, inner_puzzle_hash, coin_id
-        (list MOD_HASH (sha256 ONE MOD_HASH) TAIL_PROGRAM_HASH)
-        (a INNER_PUZZLE inner_puzzle_solution)
-        lineage_proof
-        (sha256tree INNER_PUZZLE)
-        (calculate_coin_id (f this_coin_info) (f (r this_coin_info)) (f (r (r this_coin_info))))
-        prev_coin_id    ; ID
-        this_coin_info  ; (parent_id puzzle_hash amount)
-        next_coin_proof ; (parent_id innerpuzhash amount)
-        prev_subtotal
-        extra_delta
-    )
-)
+; Coins locked with this puzzle are spendable cats.
+;
+; Choose a list of n inputs (n>=1), I_1, ... I_n with amounts A_1, ... A_n.
+;
+; We put them in a ring, so "previous" and "next" have intuitive k-1 and k+1 semantics,
+; wrapping so {n} and 0 are the same, ie. all indices are mod n.
+;
+; Each coin creates 0 or more coins with total output value O_k.
+; Let D_k = the "debt" O_k - A_k contribution of coin I_k, ie. how much debt this input accumulates.
+; Some coins may spend more than they contribute and some may spend less, ie. D_k need
+; not be zero. That's okay. It's enough for the total of all D_k in the ring to be 0.
+;
+; A coin can calculate its own D_k since it can verify A_k (it's hashed into the coin id)
+; and it can sum up `CREATE_COIN` conditions for O_k.
+;
+; Defines a "subtotal of debts" S_k for each coin as follows:
+;
+; S_1 = 0
+; S_k = S_{k-1} + D_{k-1}
+;
+; Here's the main trick that shows the ring sums to 0.
+; You can prove by induction that S_{k+1} = D_1 + D_2 + ... + D_k.
+; But it's a ring, so S_{n+1} is also S_1, which is 0. So D_1 + D_2 + ... + D_k = 0.
+; So the total debts must be 0, ie. no coins are created or destroyed.
+;
+; Each coin's solution includes I_{k-1}, I_k, and I_{k+1} along with proofs that I_{k}, and I_{k+1} are CATs of the same type.
+; Each coin's solution includes S_{k-1}. It calculates D_k = O_k - A_k, and then S_k = S_{k-1} + D_{k-1}
+;
+; Announcements are used to ensure that each S_k follows the pattern is valid.
+; Announcements automatically commit to their own coin id.
+; Coin I_k creates an announcement that further commits to I_{k-1} and S_{k-1}.
+;
+; Coin I_k gets a proof that I_{k+1} is a cat, so it knows it must also create an announcement
+; when spent. It checks that I_{k+1} creates an announcement committing to I_k and S_k.
+;
+; So S_{k+1} is correct iff S_k is correct.
+;
+; Coins also receive proofs that their neighbours are CATs, ensuring the announcements aren't forgeries.
+; Inner puzzles and the CAT layer prepend `CREATE_COIN_ANNOUNCEMENT` with different prefixes to avoid forgeries.
+; Ring announcements use 0xcb, and inner puzzles are given 0xca
+;
+; In summary, I_k generates a coin_announcement Y_k ("Y" for "yell") as follows:
+;
+;  Y_k: hash of I_k (automatically), I_{k-1}, S_k
+;
+; Each coin creates an assert_coin_announcement to ensure that the next coin's announcement is as expected:
+;  Y_{k+1} : hash of I_{k+1}, I_k, S_{k+1}
+;
+; TLDR:
+;  I_k : coins
+;  A_k : amount coin k contributes
+;  O_k : amount coin k spend
+;  D_k : difference/delta that coin k incurs (A - O)
+;  S_k : subtotal of debts D_1 + D_2 ... + D_k
+;  Y_k : announcements created by coin k committing to I_{k-1}, I_k, S_k
+;
+; All conditions go through a "transformer" that looks for CREATE_COIN conditions
+; generated by the inner solution, and wraps the puzzle hash ensuring the output is a cat.
+;
+; Three output conditions are prepended to the list of conditions for each I_k:
+;  (ASSERT_MY_ID I_k) to ensure that the passed in value for I_k is correct
+;  (CREATE_COIN_ANNOUNCEMENT I_{k-1} S_k) to create this coin's announcement
+;  (ASSERT_COIN_ANNOUNCEMENT hashed_announcement(Y_{k+1})) to ensure the next coin really is next and
+;     the relative values of S_k and S_{k+1} are correct
+;
+; This is all we need to do to ensure cats exactly balance in the inputs and outputs.
+;
+; Proof:
+;   Consider n, k, I_k values, O_k values, S_k and A_k as above.
+;   For the (CREATE_COIN_ANNOUNCEMENT Y_{k+1}) (created by the next coin)
+;   and (ASSERT_COIN_ANNOUNCEMENT hashed(Y_{k+1})) to match,
+;   we see that I_k can ensure that is has the correct value for S_{k+1}.
+;
+;   By induction, we see that S_{m+1} = sum(i, 1, m) [O_i - A_i] = sum(i, 1, m) O_i - sum(i, 1, m) A_i
+;   So S_{n+1} = sum(i, 1, n) O_i - sum(i, 1, n) A_i. But S_{n+1} is actually S_1 = 0,
+;   so thus sum(i, 1, n) O_i = sum (i, 1, n) A_i, ie. output total equals input total.
+
+;; GLOSSARY:
+;;  MOD_HASH: this code's sha256 tree hash
+;;  TAIL_PROGRAM_HASH: the program that determines if a coin can mint new cats, burn cats, and check if its lineage is valid if its parent is not a CAT
+;;  INNER_PUZZLE: an independent puzzle protecting the coins. Solutions to this puzzle are expected to generate `AGG_SIG` conditions and possibly `CREATE_COIN` conditions.
+;; ---- items above are curried into the puzzle hash ----
+;;  inner_puzzle_solution: the solution to the inner puzzle
+;;  prev_coin_id: the id for the previous coin
+;;  tail_program_reveal: reveal of TAIL_PROGRAM_HASH required to run the program if desired
+;;  tail_solution: optional solution passed into tail_program
+;;  lineage_proof: optional proof that our coin's parent is a CAT
+;;  this_coin_info: (parent_id puzzle_hash amount)
+;;  next_coin_proof: (parent_id inner_puzzle_hash amount)
+;;  prev_subtotal: the subtotal between prev-coin and this-coin
+;;  extra_delta: an amount that is added to our delta and checked by the TAIL program
+;;
+
+(mod (
+      MOD_HASH                 ;; curried into puzzle
+      TAIL_PROGRAM_HASH        ;; curried into puzzle
+      INNER_PUZZLE             ;; curried into puzzle
+      inner_puzzle_solution    ;; if invalid, INNER_PUZZLE will fail
+      lineage_proof            ;; This is the parent's coin info, used to check if the parent was a CAT. Optional if using tail_program.
+      prev_coin_id             ;; used in this coin's announcement, prev_coin ASSERT_COIN_ANNOUNCEMENT will fail if wrong
+      this_coin_info           ;; verified with ASSERT_MY_COIN_ID
+      next_coin_proof          ;; used to generate ASSERT_COIN_ANNOUNCEMENT
+      prev_subtotal            ;; included in announcement, prev_coin ASSERT_COIN_ANNOUNCEMENT will fail if wrong
+      extra_delta              ;; this is the "legal discrepancy" between your real delta and what you're announcing your delta is
+    )
+
+     ;;;;; start library code
+
+     (include condition_codes.clib)
+     (include curry-and-treehash.clib)
+     (include cat_truths.clib)
+     (include utility_macros.clib)
+
+     (defconstant RING_MORPH_BYTE 0xcb)
+
+
+    ; take two lists and merge them into one
+    (defun merge_list (list_a list_b)
+      (if list_a
+        (c (f list_a) (merge_list (r list_a) list_b))
+        list_b
+      )
+    )
+
+    ; cat_mod_struct = (MOD_HASH MOD_HASH_hash GENESIS_COIN_CHECKER GENESIS_COIN_CHECKER_hash)
+
+    (defun-inline mod_hash_from_cat_mod_struct (cat_mod_struct) (f cat_mod_struct))
+    (defun-inline mod_hash_hash_from_cat_mod_struct (cat_mod_struct) (f (r cat_mod_struct)))
+    (defun-inline tail_program_hash_from_cat_mod_struct (cat_mod_struct) (f (r (r cat_mod_struct))))
+
+     ;;;;; end library code
+
+     ;; return the puzzle hash for a cat with the given `GENESIS_COIN_CHECKER_hash` & `INNER_PUZZLE`
+     (defun-inline cat_puzzle_hash (cat_mod_struct inner_puzzle_hash)
+       (puzzle-hash-of-curried-function (mod_hash_from_cat_mod_struct cat_mod_struct)
+                                        inner_puzzle_hash
+                                        (sha256 ONE (tail_program_hash_from_cat_mod_struct cat_mod_struct))
+                                        (mod_hash_hash_from_cat_mod_struct cat_mod_struct)
+       )
+     )
+
+     ;; assert `CREATE_COIN_ANNOUNCEMENT` doesn't contain the RING_MORPH_BYTE bytes so it cannot be used to cheat the coin ring
+
+     (defun-inline morph_condition (condition cat_mod_struct)
+       (if (= (f condition) CREATE_COIN)
+         (c CREATE_COIN
+               (c (cat_puzzle_hash cat_mod_struct (f (r condition)))
+                    (r (r condition)))
+         )
+         (if (= (f condition) CREATE_COIN_ANNOUNCEMENT)
+           (assert (not (and
+                     (= 33 (strlen (f (r condition))))
+                     (= (substr (f (r condition)) 0 ONE) RING_MORPH_BYTE)  ; lazy eval
+                   ))
+             ; then
+             condition
+           )
+           condition
+         )
+       )
+     )
+
+     ;; given a coin's parent, inner_puzzle and amount, and the cat_mod_struct, calculate the id of the coin
+     (defun-inline coin_id_for_proof (coin cat_mod_struct)
+       (calculate_coin_id (f coin) (cat_puzzle_hash cat_mod_struct (f (r coin))) (f (r (r coin))))
+     )
+
+     ;; utility to fetch coin amount from coin
+     (defun-inline input_amount_for_coin (coin)
+       (f (r (r coin)))
+     )
+
+     ;; calculate the hash of an announcement
+     ;; we add 0xcb so ring announcements exist in a different namespace to announcements from inner_puzzles
+     (defun-inline calculate_annoucement_id (this_coin_id this_subtotal next_coin_id cat_mod_struct)
+       (sha256 next_coin_id RING_MORPH_BYTE (sha256tree (list this_coin_id this_subtotal)))
+     )
+
+     ;; create the `ASSERT_COIN_ANNOUNCEMENT` condition that ensures the next coin's announcement is correct
+     (defun-inline create_assert_next_announcement_condition (this_coin_id this_subtotal next_coin_id cat_mod_struct)
+       (list ASSERT_COIN_ANNOUNCEMENT
+             (calculate_annoucement_id this_coin_id
+                                            this_subtotal
+                                            next_coin_id
+                                            cat_mod_struct
+             )
+       )
+     )
+
+     ;; here we commit to I_{k-1} and S_k
+     ;; we add 0xcb so ring announcements exist in a different namespace to announcements from inner_puzzles
+     (defun-inline create_announcement_condition (prev_coin_id prev_subtotal)
+       (list CREATE_COIN_ANNOUNCEMENT
+             (concat RING_MORPH_BYTE (sha256tree (list prev_coin_id prev_subtotal)))
+       )
+      )
+
+     ;;;;;;;;;;;;;;;;;;;;;;;;;;;
+
+     ;; this function takes a condition and returns an integer indicating
+     ;; the value of all output coins created with CREATE_COIN. If it's not
+     ;; a CREATE_COIN condition, it returns 0.
+
+     (defun-inline output_value_for_condition (condition)
+       (if (= (f condition) CREATE_COIN)
+         (f (r (r condition)))
+         0
+       )
+     )
+
+     ;; add two conditions to the list of morphed conditions:
+     ;; CREATE_COIN_ANNOUNCEMENT for my announcement
+     ;; ASSERT_COIN_ANNOUNCEMENT for the next coin's announcement
+     (defun-inline generate_final_output_conditions
+       (
+         prev_subtotal
+         this_subtotal
+         morphed_conditions
+         prev_coin_id
+         this_coin_id
+         next_coin_id
+         cat_mod_struct
+       )
+         (c (create_announcement_condition prev_coin_id prev_subtotal)
+           (c (create_assert_next_announcement_condition this_coin_id this_subtotal next_coin_id cat_mod_struct)
+             morphed_conditions)
+         )
+      )
+
+
+      ;; This next section of code loops through all of the conditions to do three things:
+      ;;   1) Look for a "magic" value of -113 and, if one exists, filter it, and take note of the tail reveal and solution
+      ;;   2) Morph any CREATE_COIN or CREATE_COIN_ANNOUNCEMENT conditions
+      ;;   3) Sum the total output amount of all of the CREATE_COINs that are output by the inner puzzle
+      ;;
+      ;; After everything return a struct in the format (morphed_conditions . (output_sum . tail_reveal_and_solution))
+      ;; If multiple magic conditions are specified, the later one will take precedence
+
+      (defun-inline condition_tail_reveal (condition) (f (r (r (r condition)))))
+      (defun-inline condition_tail_solution (condition) (f (r (r (r (r condition))))))
+
+      (defun cons_onto_first_and_add_to_second (morphed_condition output_value struct)
+        (c (c morphed_condition (f struct)) (c (+ output_value (f (r struct))) (r (r struct))))
+      )
+
+      (defun find_and_strip_tail_info (inner_conditions cat_mod_struct tail_reveal_and_solution)
+        (if inner_conditions
+            (if (= (output_value_for_condition (f inner_conditions)) -113)  ; Checks this is a CREATE_COIN of value -113
+                (find_and_strip_tail_info
+                  (r inner_conditions)
+                  cat_mod_struct
+                  (c (condition_tail_reveal (f inner_conditions)) (condition_tail_solution (f inner_conditions)))
+                )
+                (cons_onto_first_and_add_to_second
+                  (morph_condition (f inner_conditions) cat_mod_struct)
+                  (output_value_for_condition (f inner_conditions))
+                  (find_and_strip_tail_info
+                    (r inner_conditions)
+                    cat_mod_struct
+                    tail_reveal_and_solution
+                  )
+                )
+            )
+            (c () (c 0 tail_reveal_and_solution))
+        )
+      )
+
+     ;;;;;;;;;;;;;;;;;;;;;;;;;;; lineage checking
+
+     ;; return true iff parent of `this_coin_info` is provably a cat
+     ;; A 'lineage proof' consists of (parent_parent_id parent_INNER_puzzle_hash parent_amount)
+     ;; We use this information to construct a coin who's puzzle has been wrapped in this MOD and verify that,
+     ;; once wrapped, it matches our parent coin's ID.
+     (defun-inline is_parent_cat (
+       cat_mod_struct
+       parent_id
+       lineage_proof
+     )
+       (= parent_id
+          (calculate_coin_id (f lineage_proof)
+                  (cat_puzzle_hash cat_mod_struct (f (r lineage_proof)))
+                  (f (r (r lineage_proof)))
+          )
+       )
+     )
+
+    (defun check_lineage_or_run_tail_program
+      (
+        this_coin_info
+        tail_reveal_and_solution
+        parent_is_cat  ; flag which says whether or not the parent CAT check ran and passed
+        lineage_proof
+        Truths
+        extra_delta
+        inner_conditions
+      )
+      (if tail_reveal_and_solution
+          (assert (= (sha256tree (f tail_reveal_and_solution)) (cat_tail_program_hash_truth Truths))
+            (merge_list
+              (a  (f tail_reveal_and_solution)
+                  (list
+                    Truths
+                    parent_is_cat
+                    lineage_proof ; Lineage proof is only guaranteed to be true if parent_is_cat
+                    extra_delta
+                    inner_conditions
+                    (r tail_reveal_and_solution)
+                  )
+              )
+              inner_conditions
+            )
+          )
+          (assert parent_is_cat (not extra_delta)
+            inner_conditions
+          )
+      )
+    )
+
+     ;;;;;;;;;;;;;;;;;;;;;;;;;;;
+
+     (defun stager_two (
+         Truths
+         (inner_conditions . (output_sum . tail_reveal_and_solution))
+         lineage_proof
+         prev_coin_id
+         this_coin_info
+         next_coin_id
+         prev_subtotal
+         extra_delta
+      )
+      (check_lineage_or_run_tail_program
+            this_coin_info
+            tail_reveal_and_solution
+            (if lineage_proof (is_parent_cat (cat_struct_truth Truths) (my_parent_cat_truth Truths) lineage_proof) ())
+            lineage_proof
+            Truths
+            extra_delta
+            (generate_final_output_conditions
+              prev_subtotal
+              ; the expression on the next line calculates `this_subtotal` by adding the delta to `prev_subtotal`
+              (+ prev_subtotal (- (input_amount_for_coin this_coin_info) output_sum) extra_delta)
+              inner_conditions
+              prev_coin_id
+              (my_id_cat_truth Truths)
+              next_coin_id
+              (cat_struct_truth Truths)
+            )
+        )
+    )
+
+    ; CAT TRUTHS struct is: ; CAT Truths is: ((Inner puzzle hash . (MOD hash . (MOD hash hash . TAIL hash))) . (my_id . (my_parent_info my_puzhash my_amount)))
+    ; create truths - this_coin_info verified true because we calculated my ID from it!
+    ; lineage proof is verified later by cat parent check or tail_program
+
+    (defun stager (
+        cat_mod_struct
+        inner_conditions
+        lineage_proof
+        inner_puzzle_hash
+        my_id
+        prev_coin_id
+        this_coin_info
+        next_coin_proof
+        prev_subtotal
+        extra_delta
+     )
+      (c (list ASSERT_MY_COIN_ID my_id) (stager_two
+        (cat_truth_data_to_truth_struct
+          inner_puzzle_hash
+          cat_mod_struct
+          my_id
+          this_coin_info
+        )
+        (find_and_strip_tail_info inner_conditions cat_mod_struct ())
+        lineage_proof
+        prev_coin_id
+        this_coin_info
+        (coin_id_for_proof next_coin_proof cat_mod_struct)
+        prev_subtotal
+        extra_delta
+      ))
+    )
+
+    (stager
+        ;; calculate cat_mod_struct, inner_puzzle_hash, coin_id
+        (list MOD_HASH (sha256 ONE MOD_HASH) TAIL_PROGRAM_HASH)
+        (a INNER_PUZZLE inner_puzzle_solution)
+        lineage_proof
+        (sha256tree INNER_PUZZLE)
+        (calculate_coin_id (f this_coin_info) (f (r this_coin_info)) (f (r (r this_coin_info))))
+        prev_coin_id    ; ID
+        this_coin_info  ; (parent_id puzzle_hash amount)
+        next_coin_proof ; (parent_id innerpuzhash amount)
+        prev_subtotal
+        extra_delta
+    )
+)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/cat_v2.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/chialisp_deserialisation.clsp`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/chialisp_deserialisation.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/condition_codes.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/condition_codes.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/create-lock-puzzlehash.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/create-lock-puzzlehash.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry-and-treehash.clinc` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/curry-and-treehash.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry.clib` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/curry.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/delegated_tail.clsp`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-; This is a "limitations_program" for use with cat.clvm.
+; This is a "limitations_program" for use with cat.clsp.
 (mod (
       PUBKEY
       Truths
       parent_is_cat
       lineage_proof
       delta
       inner_conditions
       (
         delegated_puzzle
         delegated_solution
       )
     )
 
-    (include condition_codes.clvm)
+    (include condition_codes.clib)
 
     (defun sha256tree1 (TREE)
           (if (l TREE)
               (sha256 2 (sha256tree1 (f TREE)) (sha256tree1 (r TREE)))
               (sha256 1 TREE)))
 
     (c (list AGG_SIG_UNSAFE PUBKEY (sha256tree1 delegated_puzzle))
       (a delegated_puzzle (c Truths (c parent_is_cat (c lineage_proof (c delta (c inner_conditions delegated_solution))))))
     )
-)
+)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/did_innerpuz.clsp`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
   my_id  ; my coin ID
   )
   ;message is the new puzzle in the recovery and standard spend cases
 
   ;MOD_HASH, MY_PUBKEY, RECOVERY_DID_LIST_HASH are curried into the puzzle
   ;EXAMPLE SOLUTION (0xcafef00d 0x12341234 0x923bf9a7856b19d335a65f12d68957d497e1f0c16c0e14baf6d120e60753a1ce 2 1 100 (q "source code") 0xdeadbeef 0xcafef00d ((0xdadadada 0xdad5dad5 200) () (0xfafafafa 0xfaf5faf5 200)) 0xfadeddab (0x22222222 0x33333333 0x44444444))
 
-  (include condition_codes.clvm)
-  (include curry-and-treehash.clinc)
+  (include condition_codes.clib)
+  (include curry-and-treehash.clib)
 
   ; takes a lisp tree and returns the hash of it
   (defun sha256tree1 (TREE)
       (if (l TREE)
           (sha256 2 (sha256tree1 (f TREE)) (sha256tree1 (r TREE)))
           (sha256 1 TREE)
       )
@@ -48,15 +48,15 @@
   ; this function calculates a coin ID given the inner puzzle and singleton information
   (defun create_coin_ID_for_recovery (SINGLETON_STRUCT launcher_id parent innerpuzhash amount)
     (sha256 parent (calculate_full_puzzle_hash (c (f SINGLETON_STRUCT) (c launcher_id (r (r SINGLETON_STRUCT)))) innerpuzhash) amount)
   )
 
 
   ; return the full puzzlehash for a singleton with the innerpuzzle curried in
-  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clinc
+  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clib
   (defun-inline calculate_full_puzzle_hash (SINGLETON_STRUCT inner_puzzle_hash)
      (puzzle-hash-of-curried-function (f SINGLETON_STRUCT)
                                       inner_puzzle_hash
                                       (sha256tree1 SINGLETON_STRUCT)
      )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/did_innerpuz.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/genesis_by_coin_id.clsp`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/genesis_by_puzzle_hash.clsp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-; This is a "limitations_program" for use with cat.clvm.
+; This is a "limitations_program" for use with cat.clsp.
 ;
 ; This checker allows new CATs to be created if their parent has a particular puzzle hash
 (mod (
       GENESIS_PUZZLE_HASH
       Truths
       parent_is_cat
       lineage_proof
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/graftroot_dl_offers.clsp`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     proofs_of_inclusion
     new_metadatas  ; (root . etc)
     new_metadata_updaters
     new_inner_puzs
     inner_solution
   )
 
-  (include condition_codes.clvm)
+  (include condition_codes.clib)
   (include merkle_utils.clib)
-  (include curry-and-treehash.clinc)
+  (include curry-and-treehash.clib)
 
   (defmacro assert items
       (if (r items)
           (list if (f items) (c assert (r items)) (q . (x)))
           (f items)
       )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/graftroot_dl_offers.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/json.clib` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/json.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/load_clvm.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/load_clvm.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         compile_clvm_in_lock(full_path, output, search_paths)
 
 
 def load_serialized_clvm(
     clvm_filename, package_or_requirement=__name__, include_standard_libraries: bool = False, recompile: bool = True
 ) -> SerializedProgram:
     """
-    This function takes a .clvm file in the given package and compiles it to a
-    .clvm.hex file if the .hex file is missing or older than the .clvm file, then
+    This function takes a .clsp file in the given package and compiles it to a
+    .clsp.hex file if the .hex file is missing or older than the .clsp file, then
     returns the contents of the .hex file as a `Program`.
 
     clvm_filename: file name
     package_or_requirement: usually `__name__` if the clvm file is in the same package
     """
     hex_filename = f"{clvm_filename}.hex"
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/merkle_utils.clib` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/merkle_utils.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_metadata_updater_default.clsp`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_metadata_updater_updateable.clsp`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_layer.clsp`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     NFT_OWNERSHIP_LAYER_MOD_HASH
     CURRENT_OWNER
     TRANSFER_PROGRAM
     INNER_PUZZLE
     inner_solution
    )
 
-   (include condition_codes.clvm)
-   (include curry-and-treehash.clinc)
+   (include condition_codes.clib)
+   (include curry-and-treehash.clib)
    (include utility_macros.clib)
 
    (defconstant NEW_OWNER_CONDITION -10)
    (defconstant ANNOUNCEMENT_PREFIX 0xad4c)  ; first 2 bytes of (sha256 "Ownership Layer")
 
    (defun-inline nft_ownership_layer_puzzle_hash (NFT_OWNERSHIP_LAYER_MOD_HASH new_owner TRANSFER_PROGRAM inner_puzzle_hash)
       (puzzle-hash-of-curried-function NFT_OWNERSHIP_LAYER_MOD_HASH
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_layer.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clsp`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     Current_Owner  ; Truth
     conditions  ; Truth
     solution  ; created from the NFT's inner puzzle - solution is (new_owner trade_prices_list new_did_inner_hash)
   )
 
   ; This is a transfer program - which must return (new_owner, Optional[new_transfer_program], conditions)
 
-  (include condition_codes.clvm)
-  (include curry-and-treehash.clinc)
+  (include condition_codes.clib)
+  (include curry-and-treehash.clib)
 
   (defconstant TEN_THOUSAND 10000)
 
   ;; return the full puzzlehash for a singleton with the innerpuzzle curried in
-  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clinc
+  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clib
   (defun-inline calculate_full_puzzle_hash (SINGLETON_STRUCT inner_puzzle_hash)
      (puzzle-hash-of-curried-function (f SINGLETON_STRUCT)
                                       inner_puzzle_hash
                                       (sha256tree SINGLETON_STRUCT)
      )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_state_layer.clsp`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     NFT_STATE_LAYER_MOD_HASH
     METADATA
     METADATA_UPDATER_PUZZLE_HASH
     INNER_PUZZLE
     inner_solution
   )
 
-  (include condition_codes.clvm)
-  (include curry-and-treehash.clinc)
+  (include condition_codes.clib)
+  (include curry-and-treehash.clib)
   (include utility_macros.clib)
 
   (defun-inline nft_state_layer_puzzle_hash (NFT_STATE_LAYER_MOD_HASH METADATA METADATA_UPDATER_PUZZLE_HASH inner_puzzle_hash)
     (puzzle-hash-of-curried-function NFT_STATE_LAYER_MOD_HASH
                                      inner_puzzle_hash
                                      (sha256 ONE METADATA_UPDATER_PUZZLE_HASH)
                                      (sha256tree METADATA)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/nft_state_layer.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from __future__ import annotations
 
 from chia.types.blockchain_format.program import Program
 
 from .load_clvm import load_clvm_maybe_recompile
 
-MOD = load_clvm_maybe_recompile("p2_conditions.clvm")
+MOD = load_clvm_maybe_recompile("p2_conditions.clsp")
 
 
 def puzzle_for_conditions(conditions) -> Program:
     return MOD.run([conditions])
 
 
 def solution_for_conditions(conditions) -> Program:
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from __future__ import annotations
 
 from chia.types.blockchain_format.program import Program
 
 from .load_clvm import load_clvm_maybe_recompile
 
-MOD = load_clvm_maybe_recompile("p2_delegated_conditions.clvm")
+MOD = load_clvm_maybe_recompile("p2_delegated_conditions.clsp")
 
 
 def puzzle_for_pk(public_key: Program) -> Program:
     return MOD.curry(public_key)
 
 
 def solution_for_conditions(conditions: Program) -> Program:
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 
 from chia.types.blockchain_format.program import Program
 
 from . import p2_conditions
 from .load_clvm import load_clvm_maybe_recompile
 
-MOD = load_clvm_maybe_recompile("p2_delegated_puzzle.clvm")
+MOD = load_clvm_maybe_recompile("p2_delegated_puzzle.clsp")
 
 
 def puzzle_for_pk(public_key: bytes) -> Program:
     return MOD.curry(public_key)
 
 
 def solution_for_conditions(conditions) -> Program:
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clsp`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     (defmacro assert items
         (if (r items)
             (list if (f items) (c assert (r items)) (q . (x)))
             (f items)
         )
     )
 
-    (include condition_codes.clvm)
+    (include condition_codes.clib)
 
     ;; hash a tree
     ;; This is used to calculate a puzzle hash given a puzzle program.
     (defun sha256tree1
            (TREE)
            (if (l TREE)
                (sha256 2 (sha256tree1 (f TREE)) (sha256tree1 (r TREE)))
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 from .load_clvm import load_clvm_maybe_recompile
 from .p2_conditions import puzzle_for_conditions
 
 DEFAULT_HIDDEN_PUZZLE = Program.from_bytes(bytes.fromhex("ff0980"))
 
 DEFAULT_HIDDEN_PUZZLE_HASH = DEFAULT_HIDDEN_PUZZLE.get_tree_hash()  # this puzzle `(x)` always fails
 
-MOD = load_clvm_maybe_recompile("p2_delegated_puzzle_or_hidden_puzzle.clvm")
+MOD = load_clvm_maybe_recompile("p2_delegated_puzzle_or_hidden_puzzle.clsp")
 
 QUOTED_MOD_HASH = calculate_hash_of_quoted_mod_hash(MOD.get_tree_hash())
 
 PublicKeyProgram = Union[bytes, Program]
 
 GROUP_ORDER = 0x73EDA753299D7D483339D80809A1D80553BDA402FFFE5BFEFFFFFFFF00000001
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clsp`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ;  solution: the solution to the delegated puzzle
 
 
 (mod
     (M public_key_list selectors delegated_puzzle solution)
 
-    (include condition_codes.clvm)
+    (include condition_codes.clib)
 
     ;; hash a tree
     ;; This is used to calculate a puzzle hash given a puzzle program.
     (defun sha256tree1
            (TREE)
            (if (l TREE)
                (sha256 2 (sha256tree1 (f TREE)) (sha256tree1 (r TREE)))
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from __future__ import annotations
 
 from chia.types.blockchain_format.program import Program
 
 from .load_clvm import load_clvm_maybe_recompile
 
-MOD = load_clvm_maybe_recompile("p2_m_of_n_delegate_direct.clvm")
+MOD = load_clvm_maybe_recompile("p2_m_of_n_delegate_direct.clsp")
 
 
 def puzzle_for_m_of_public_key_list(m, public_key_list) -> Program:
     return MOD.curry(m, public_key_list)
 
 
 def solution_for_delegated_puzzle(m, selectors, puzzle, solution) -> Program:
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_puzzle_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from __future__ import annotations
 
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 
 from .load_clvm import load_clvm_maybe_recompile
 
-MOD = load_clvm_maybe_recompile("p2_puzzle_hash.clvm")
+MOD = load_clvm_maybe_recompile("p2_puzzle_hash.clsp")
 
 
 def puzzle_for_inner_puzzle_hash(inner_puzzle_hash: bytes32) -> Program:
     program = MOD.curry(inner_puzzle_hash)
     return program
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton.clsp`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
   ; SINGLETON_MOD_HASH is the mod-hash for the singleton_top_layer puzzle
   ; LAUNCHER_ID is the ID of the singleton we are committed to paying to
   ; LAUNCHER_PUZZLE_HASH is the puzzle hash of the launcher
   ; singleton_inner_puzzle_hash is the innerpuzzlehash for our singleton at the current time
   ; my_id is the coin_id of the coin that this puzzle is locked into
 
-  (include condition_codes.clvm)
-  (include curry-and-treehash.clinc)
+  (include condition_codes.clib)
+  (include curry-and-treehash.clib)
 
   ;; return the full puzzlehash for a singleton with the innerpuzzle curried in
-  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clinc
+  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clib
   (defun-inline calculate_full_puzzle_hash (SINGLETON_MOD_HASH LAUNCHER_ID LAUNCHER_PUZZLE_HASH inner_puzzle_hash)
      (puzzle-hash-of-curried-function SINGLETON_MOD_HASH
                                       inner_puzzle_hash
                                       (sha256tree (c SINGLETON_MOD_HASH (c LAUNCHER_ID LAUNCHER_PUZZLE_HASH)))
      )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clsp`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,29 @@
   ; SECONDS_DELAY is the number of seconds before the coin can be spent with `DELAYED_PUZZLE_HASH`
   ; DELAYED_PUZZLE_HASH is the puzzle hash of the delayed puzzle
   ; if my_id is passed in as () then this signals that we are trying to do a delayed spend case
   ; p1's meaning changes depending upon which case we're using
     ; if we are paying to singleton then p1 is singleton_inner_puzzle_hash
     ; if we are running the delayed case then p1 is the amount to output
 
-  (include condition_codes.clvm)
-  (include curry-and-treehash.clinc)
+  (include condition_codes.clib)
+  (include curry-and-treehash.clib)
 
   ;; return the full puzzlehash for a singleton with the innerpuzzle curried in
-  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clinc
+  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clib
   (defun-inline delayed_spend (SECONDS_DELAY DELAYED_PUZZLE_HASH amount)
     (list
       (list ASSERT_SECONDS_RELATIVE SECONDS_DELAY)
       (list CREATE_COIN DELAYED_PUZZLE_HASH amount)
       (list ASSERT_MY_AMOUNT amount)
     )
   )
 
   ;; return the full puzzlehash for a singleton with the innerpuzzle curried in
-  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clinc
+  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clib
   (defun-inline calculate_full_puzzle_hash (SINGLETON_MOD_HASH LAUNCHER_ID LAUNCHER_PUZZLE_HASH inner_puzzle_hash)
      (puzzle-hash-of-curried-function SINGLETON_MOD_HASH
                                       inner_puzzle_hash
                                       (sha256tree (c SINGLETON_MOD_HASH (c LAUNCHER_ID LAUNCHER_PUZZLE_HASH)))
      )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_member_innerpuz.clsp`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   ; p1 is pool_reward_amount if absorbing money
   ; p1 is extra_data key_value_list if escaping
 
   ; pool_reward_amount is the value of the coin reward - this is passed in so that this puzzle will still work after halvenings
   ; pool_reward_height is the block height that the reward was generated at. This is used to calculate the coin ID.
   ; key_value_list is signed extra data that the wallet may want to publicly announce for syncing purposes
 
-  (include condition_codes.clvm)
+  (include condition_codes.clib)
   (include singleton_truths.clib)
 
   ; takes a lisp tree and returns the hash of it
   (defun sha256tree (TREE)
       (if (l TREE)
           (sha256 2 (sha256tree (f TREE)) (sha256tree (r TREE)))
           (sha256 1 TREE)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_member_innerpuz.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_waitingroom_innerpuz.clsp`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   ; if spend_type is 0
     ; p1 is pool_reward_amount - the value of the coin reward - this is passed in so that this puzzle will still work after halvenings
     ; p2 is pool_reward_height - the block height that the reward was generated at. This is used to calculate the coin ID.
   ; if spend_type is 1
     ; p1 is extra_data key_value_list - signed extra data that the wallet may want to publicly announce for syncing purposes
     ; p2 is destination_puzhash - the location that the escape spend wants to create itself to
 
-  (include condition_codes.clvm)
+  (include condition_codes.clib)
   (include singleton_truths.clib)
 
   ; takes a lisp tree and returns the hash of it
   (defun sha256tree (TREE)
       (if (l TREE)
           (sha256 2 (sha256tree (f TREE)) (sha256tree (r TREE)))
           (sha256 1 TREE)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/pool_waitingroom_innerpuz.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/make_prefarm_ph.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/prefarm/make_prefarm_ph.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/spend_prefarm.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/prefarm/spend_prefarm.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/puzzle_utils.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/puzzle_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/rom_bootstrap_generator.clsp`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 (mod (block_decompresser_program (historical_blocks_tree))
 
     (defconstant local_deserialize_mod
-        ;; this monstrosity is the assembly output of `chialisp_deserialisation.clvm`
+        ;; this monstrosity is the assembly output of `chialisp_deserialisation.clsp`
         ;; it's pasted in here because the compiler doesn't yet support nested `mod`
         ;; my apologies -- RK
 
         (a (q 5 (a 62 (c 2 (c 5 ()))))
            (c (q ((-1 . 127) -33 . -65) ((a (i (= 11 (q . -128)) (q 4 () (c 5 ())) (q 2 (i (>s 11 24) (q 2 26 (c 2 (c (a (i (>s 11 28) (q 2 (i (>s 11 20) (q 8) (q 4 (concat (logand (q . 31) 11) (substr 5 () (q . 1))) (c (substr 5 (q . 1)) ()))) 1) (q 4 (logand (q . 63) 11) (c 5 ()))) 1) ()))) (q 4 11 (c 5 ()))) 1)) 1) 4 (substr 21 () 9) (c (substr 21 9) ())) (c (c 5 19) (c 43 ())) (a 22 (c 2 (c 9 (c (a 62 (c 2 (c 21 ()))) ())))) 2 (i (= (substr 5 () (q . 1)) 16) (q 2 46 (c 2 (c (a 62 (c 2 (c (substr 5 (q . 1)) ()))) ()))) (q 2 18 (c 2 (c (substr 5 (q . 1)) (c (substr 5 () (q . 1)) ()))))) 1)
               1))
     )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/rom_bootstrap_generator.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments.clsp`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   ;; `notarized_payments` is a list of notarized coin payments
   ;; a notarized coin payment is `(nonce . ((puzzle_hash amount ...) (puzzle_hash amount ...) ...))`
   ;; Each notarized coin payment creates some `(CREATE_COIN puzzle_hash amount ...)` payments
   ;; and a `(CREATE_PUZZLE_ANNOUNCEMENT (sha256tree notarized_coin_payment))` announcement
   ;; The idea is the other side of this trade requires observing the announcement from a
   ;; `settlement_payments` puzzle hash as a condition of one or more coin spends.
 
-  (include condition_codes.clvm)
+  (include condition_codes.clib)
   (include utility_macros.clib)
 
   (defun sha256tree (TREE)
      (if (l TREE)
          (sha256 2 (sha256tree (f TREE)) (sha256tree (r TREE)))
          (sha256 1 TREE)
      )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments_old.clsp`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   ;; `notarized_payments` is a list of notarized coin payments
   ;; a notarized coin payment is `(nonce . ((puzzle_hash amount ...) (puzzle_hash amount ...) ...))`
   ;; Each notarized coin payment creates some `(CREATE_COIN puzzle_hash amount ...)` payments
   ;; and a `(CREATE_PUZZLE_ANNOUNCEMENT (sha256tree notarized_coin_payment))` announcement
   ;; The idea is the other side of this trade requires observing the announcement from a
   ;; `settlement_payments` puzzle hash as a condition of one or more coin spends.
 
-  (include condition_codes.clvm)
+  (include condition_codes.clib)
 
   (defun sha256tree (TREE)
      (if (l TREE)
          (sha256 2 (sha256tree (f TREE)) (sha256tree (r TREE)))
          (sha256 1 TREE)
      )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/settlement_payments_old.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer.clsp`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 ; EXAMPLE SOLUTION '(0xfadeddab 0xdeadbeef 1 (0xdeadbeef 200) 50 ((51 0xfadeddab 100) (60 "trash") (51 deadbeef 0)))'
 
 
 ; This puzzle is a wrapper around an inner smart puzzle which guarantees uniqueness.
 ; It takes its singleton identity from a coin with a launcher puzzle which guarantees that it is unique.
 
-  (include condition_codes.clvm)
-  (include curry-and-treehash.clinc)
+  (include condition_codes.clib)
+  (include curry-and-treehash.clib)
   (include singleton_truths.clib)
 
   ; takes a lisp tree and returns the hash of it
   (defun sha256tree1 (TREE)
       (if (l TREE)
           (sha256 2 (sha256tree1 (f TREE)) (sha256tree1 (r TREE)))
           (sha256 1 TREE)
@@ -35,15 +35,15 @@
   )
 
   (defun-inline mod_hash_for_singleton_struct (SINGLETON_STRUCT) (f SINGLETON_STRUCT))
   (defun-inline launcher_id_for_singleton_struct (SINGLETON_STRUCT) (f (r SINGLETON_STRUCT)))
   (defun-inline launcher_puzzle_hash_for_singleton_struct (SINGLETON_STRUCT) (r (r SINGLETON_STRUCT)))
 
   ;; return the full puzzlehash for a singleton with the innerpuzzle curried in
-  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clinc
+  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clib
   (defun-inline calculate_full_puzzle_hash (SINGLETON_STRUCT inner_puzzle_hash)
      (puzzle-hash-of-curried-function (mod_hash_for_singleton_struct SINGLETON_STRUCT)
                                       inner_puzzle_hash
                                       (sha256tree1 SINGLETON_STRUCT)
      )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from chia.types.coin_spend import CoinSpend
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.util.hash import std_hash
 from chia.util.ints import uint64
 from chia.wallet.lineage_proof import LineageProof
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 
-SINGLETON_MOD = load_clvm_maybe_recompile("singleton_top_layer.clvm")
+SINGLETON_MOD = load_clvm_maybe_recompile("singleton_top_layer.clsp")
 SINGLETON_MOD_HASH = SINGLETON_MOD.get_tree_hash()
-P2_SINGLETON_MOD = load_clvm_maybe_recompile("p2_singleton.clvm")
-P2_SINGLETON_OR_DELAYED_MOD = load_clvm_maybe_recompile("p2_singleton_or_delayed_puzhash.clvm")
-SINGLETON_LAUNCHER = load_clvm_maybe_recompile("singleton_launcher.clvm")
+P2_SINGLETON_MOD = load_clvm_maybe_recompile("p2_singleton.clsp")
+P2_SINGLETON_OR_DELAYED_MOD = load_clvm_maybe_recompile("p2_singleton_or_delayed_puzhash.clsp")
+SINGLETON_LAUNCHER = load_clvm_maybe_recompile("singleton_launcher.clsp")
 SINGLETON_LAUNCHER_HASH = SINGLETON_LAUNCHER.get_tree_hash()
 ESCAPE_VALUE = -113
 MELT_CONDITION = [ConditionOpcode.CREATE_COIN, 0, ESCAPE_VALUE]
 
 
 #
 # An explanation of how this functions from a user's perspective
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer_v1_1.clsp`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 ; EXAMPLE SOLUTION '(0xfadeddab 0xdeadbeef 1 (0xdeadbeef 200) 50 ((51 0xfadeddab 100) (60 "trash") (51 deadbeef 0)))'
 
 
 ; This puzzle is a wrapper around an inner smart puzzle which guarantees uniqueness.
 ; It takes its singleton identity from a coin with a launcher puzzle which guarantees that it is unique.
 
-  (include condition_codes.clvm)
-  (include curry-and-treehash.clinc)  ; also imports the constant ONE == 1
+  (include condition_codes.clib)
+  (include curry-and-treehash.clib)  ; also imports the constant ONE == 1
   (include singleton_truths.clib)
   (include utility_macros.clib)
 
   (defun-inline mod_hash_for_singleton_struct (SINGLETON_STRUCT) (f SINGLETON_STRUCT))
   (defun-inline launcher_id_for_singleton_struct (SINGLETON_STRUCT) (f (r SINGLETON_STRUCT)))
   (defun-inline launcher_puzzle_hash_for_singleton_struct (SINGLETON_STRUCT) (r (r SINGLETON_STRUCT)))
 
   ;; return the full puzzlehash for a singleton with the innerpuzzle curried in
-  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clinc
+  ; puzzle-hash-of-curried-function is imported from curry-and-treehash.clib
   (defun-inline calculate_full_puzzle_hash (SINGLETON_STRUCT inner_puzzle_hash)
      (puzzle-hash-of-curried-function (mod_hash_for_singleton_struct SINGLETON_STRUCT)
                                       inner_puzzle_hash
                                       (sha256tree SINGLETON_STRUCT)
      )
   )
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer_v1_1.clsp.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_top_layer_v1_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.util.hash import std_hash
 from chia.util.ints import uint64
 from chia.wallet.lineage_proof import LineageProof
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.uncurried_puzzle import UncurriedPuzzle
 
-SINGLETON_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clvm")
+SINGLETON_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clsp")
 SINGLETON_MOD_HASH = SINGLETON_MOD.get_tree_hash()
-P2_SINGLETON_MOD = load_clvm_maybe_recompile("p2_singleton.clvm")
-P2_SINGLETON_OR_DELAYED_MOD = load_clvm_maybe_recompile("p2_singleton_or_delayed_puzhash.clvm")
-SINGLETON_LAUNCHER = load_clvm_maybe_recompile("singleton_launcher.clvm")
+P2_SINGLETON_MOD = load_clvm_maybe_recompile("p2_singleton.clsp")
+P2_SINGLETON_OR_DELAYED_MOD = load_clvm_maybe_recompile("p2_singleton_or_delayed_puzhash.clsp")
+SINGLETON_LAUNCHER = load_clvm_maybe_recompile("singleton_launcher.clsp")
 SINGLETON_LAUNCHER_HASH = SINGLETON_LAUNCHER.get_tree_hash()
 ESCAPE_VALUE = -113
 MELT_CONDITION = [ConditionOpcode.CREATE_COIN, 0, ESCAPE_VALUE]
 
 
 #
 # An explanation of how this functions from a user's perspective
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_truths.clib` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/singleton_truths.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/tails.py` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/tails.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 )
 from chia.wallet.cat_wallet.lineage_store import CATLineageStore
 from chia.wallet.lineage_proof import LineageProof
 from chia.wallet.puzzles.cat_loader import CAT_MOD
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.transaction_record import TransactionRecord
 
-GENESIS_BY_ID_MOD = load_clvm_maybe_recompile("genesis_by_coin_id.clvm")
-GENESIS_BY_PUZHASH_MOD = load_clvm_maybe_recompile("genesis_by_puzzle_hash.clvm")
-EVERYTHING_WITH_SIG_MOD = load_clvm_maybe_recompile("everything_with_signature.clvm")
-DELEGATED_LIMITATIONS_MOD = load_clvm_maybe_recompile("delegated_tail.clvm")
+GENESIS_BY_ID_MOD = load_clvm_maybe_recompile("genesis_by_coin_id.clsp")
+GENESIS_BY_PUZHASH_MOD = load_clvm_maybe_recompile("genesis_by_puzzle_hash.clsp")
+EVERYTHING_WITH_SIG_MOD = load_clvm_maybe_recompile("everything_with_signature.clsp")
+DELEGATED_LIMITATIONS_MOD = load_clvm_maybe_recompile("delegated_tail.clsp")
 
 
 class LimitationsProgram:
     @staticmethod
     def match(uncurried_mod: Program, curried_args: Program) -> Tuple[bool, List[Program]]:
         raise NotImplementedError("Need to implement 'match' on limitations programs")
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm` & `chia-blockchain-1.8.0rc1/chia/wallet/puzzles/test_multiple_generator_input_arguments.clsp`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/secret_key_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/secret_key_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/sign_coin_spends.py` & `chia-blockchain-1.8.0rc1/chia/wallet/sign_coin_spends.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/singleton.py` & `chia-blockchain-1.8.0rc1/chia/wallet/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import Optional
 
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.util.curry_and_treehash import calculate_hash_of_quoted_mod_hash, curry_and_treehash
 
-SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clvm")
+SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clsp")
 SINGLETON_TOP_LAYER_MOD_HASH = SINGLETON_TOP_LAYER_MOD.get_tree_hash()
 SINGLETON_TOP_LAYER_MOD_HASH_QUOTED = calculate_hash_of_quoted_mod_hash(SINGLETON_TOP_LAYER_MOD_HASH)
-SINGLETON_LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clvm")
+SINGLETON_LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clsp")
 SINGLETON_LAUNCHER_PUZZLE_HASH = SINGLETON_LAUNCHER_PUZZLE.get_tree_hash()
 
 
 def get_inner_puzzle_from_singleton(puzzle: Program) -> Optional[Program]:
     """
     Extract the inner puzzle of a singleton
     :param puzzle: Singleton puzzle
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/trade_manager.py` & `chia-blockchain-1.8.0rc1/chia/wallet/trade_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 from chia.wallet.trading.trade_store import TradeStore
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.util.transaction_type import TransactionType
 from chia.wallet.util.wallet_types import WalletType
 from chia.wallet.wallet import Wallet
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 
-OFFER_MOD = load_clvm_maybe_recompile("settlement_payments.clvm")
+OFFER_MOD = load_clvm_maybe_recompile("settlement_payments.clsp")
 
 
 class TradeManager:
     """
-    This class is a driver for creating and accepting settlement_payments.clvm style offers.
+    This class is a driver for creating and accepting settlement_payments.clsp style offers.
 
     By default, standard XCH is supported but to support other types of assets you must implement certain functions on
     the asset's wallet as well as create a driver for its puzzle(s).  Here is a guide to integrating a new types of
     assets with this trade manager:
 
     Puzzle Drivers:
       - See chia/wallet/outer_puzzles.py for a full description of how to build these
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/trade_record.py` & `chia-blockchain-1.8.0rc1/chia/wallet/trade_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/trading/offer.py` & `chia-blockchain-1.8.0rc1/chia/wallet/trading/offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 from chia.wallet.uncurried_puzzle import UncurriedPuzzle, uncurry_puzzle
 from chia.wallet.util.puzzle_compression import (
     compress_object_with_puzzles,
     decompress_object_with_puzzles,
     lowest_best_version,
 )
 
-OFFER_MOD_OLD = load_clvm_maybe_recompile("settlement_payments_old.clvm")
-OFFER_MOD = load_clvm_maybe_recompile("settlement_payments.clvm")
+OFFER_MOD_OLD = load_clvm_maybe_recompile("settlement_payments_old.clsp")
+OFFER_MOD = load_clvm_maybe_recompile("settlement_payments.clsp")
 OFFER_MOD_OLD_HASH = OFFER_MOD_OLD.get_tree_hash()
 OFFER_MOD_HASH = OFFER_MOD.get_tree_hash()
 ZERO_32 = bytes32([0] * 32)
 
 
 def detect_dependent_coin(
     names: List[bytes32], deps: Dict[bytes32, List[bytes32]], announcement_dict: Dict[bytes32, List[bytes32]]
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/trading/trade_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/trading/trade_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/transaction_record.py` & `chia-blockchain-1.8.0rc1/chia/wallet/transaction_record.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from chia.util.errors import Err
 from chia.util.ints import uint8, uint32, uint64
 from chia.util.streamable import Streamable, streamable
 from chia.wallet.util.transaction_type import TransactionType
 
 T = TypeVar("T")
 
+minimum_send_attempts = 6
+
 
 @dataclass
 class ItemAndTransactionRecords(Generic[T]):
     item: T
     transaction_records: List["TransactionRecord"]
 
 
@@ -108,18 +110,17 @@
             for coin_id, memos in self.get_memos().items()
             for memo in memos
             if memo is not None
         }
         return formatted
 
     def is_valid(self) -> bool:
-        past_receipts = self.sent_to
-        if len(past_receipts) < 6:
+        if len(self.sent_to) < minimum_send_attempts:
             # we haven't tried enough peers yet
             return True
-        if any([x[0] for x in past_receipts if x[0] == MempoolInclusionStatus.SUCCESS.value]):
+        if any(x[1] == MempoolInclusionStatus.SUCCESS for x in self.sent_to):
             # we managed to push it to mempool at least once
             return True
-        if any([x[1] for x in past_receipts if x[1] in (Err.INVALID_FEE_LOW_FEE, Err.INVALID_FEE_TOO_CLOSE_TO_ZERO)]):
+        if any(x[2] in (Err.INVALID_FEE_LOW_FEE.name, Err.INVALID_FEE_TOO_CLOSE_TO_ZERO.name) for x in self.sent_to):
             # we tried to push it to mempool and got a fee error so it's a temporary error
             return True
         return False
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/address_type.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/address_type.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/compute_hints.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/compute_hints.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/compute_memos.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/compute_memos.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/curry_and_treehash.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/curry_and_treehash.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/debug_spend_bundle.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/debug_spend_bundle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/json_clvm_utils.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/json_clvm_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/merkle_tree.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/merkle_utils.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/merkle_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/new_peak_queue.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/new_peak_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/peer_request_cache.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/peer_request_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/puzzle_compression.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/puzzle_compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 
 # Need the legacy CAT mod for zlib backwards compatibility
 LEGACY_CAT_MOD = Program.fromhex(
     "ff02ffff01ff02ff5effff04ff02ffff04ffff04ff05ffff04ffff0bff2cff0580ffff04ff0bff80808080ffff04ffff02ff17ff2f80ffff04ff5fffff04ffff02ff2effff04ff02ffff04ff17ff80808080ffff04ffff0bff82027fff82057fff820b7f80ffff04ff81bfffff04ff82017fffff04ff8202ffffff04ff8205ffffff04ff820bffff80808080808080808080808080ffff04ffff01ffffffff81ca3dff46ff0233ffff3c04ff01ff0181cbffffff02ff02ffff03ff05ffff01ff02ff32ffff04ff02ffff04ff0dffff04ffff0bff22ffff0bff2cff3480ffff0bff22ffff0bff22ffff0bff2cff5c80ff0980ffff0bff22ff0bffff0bff2cff8080808080ff8080808080ffff010b80ff0180ffff02ffff03ff0bffff01ff02ffff03ffff09ffff02ff2effff04ff02ffff04ff13ff80808080ff820b9f80ffff01ff02ff26ffff04ff02ffff04ffff02ff13ffff04ff5fffff04ff17ffff04ff2fffff04ff81bfffff04ff82017fffff04ff1bff8080808080808080ffff04ff82017fff8080808080ffff01ff088080ff0180ffff01ff02ffff03ff17ffff01ff02ffff03ffff20ff81bf80ffff0182017fffff01ff088080ff0180ffff01ff088080ff018080ff0180ffff04ffff04ff05ff2780ffff04ffff10ff0bff5780ff778080ff02ffff03ff05ffff01ff02ffff03ffff09ffff02ffff03ffff09ff11ff7880ffff0159ff8080ff0180ffff01818f80ffff01ff02ff7affff04ff02ffff04ff0dffff04ff0bffff04ffff04ff81b9ff82017980ff808080808080ffff01ff02ff5affff04ff02ffff04ffff02ffff03ffff09ff11ff7880ffff01ff04ff78ffff04ffff02ff36ffff04ff02ffff04ff13ffff04ff29ffff04ffff0bff2cff5b80ffff04ff2bff80808080808080ff398080ffff01ff02ffff03ffff09ff11ff2480ffff01ff04ff24ffff04ffff0bff20ff2980ff398080ffff010980ff018080ff0180ffff04ffff02ffff03ffff09ff11ff7880ffff0159ff8080ff0180ffff04ffff02ff7affff04ff02ffff04ff0dffff04ff0bffff04ff17ff808080808080ff80808080808080ff0180ffff01ff04ff80ffff04ff80ff17808080ff0180ffffff02ffff03ff05ffff01ff04ff09ffff02ff26ffff04ff02ffff04ff0dffff04ff0bff808080808080ffff010b80ff0180ff0bff22ffff0bff2cff5880ffff0bff22ffff0bff22ffff0bff2cff5c80ff0580ffff0bff22ffff02ff32ffff04ff02ffff04ff07ffff04ffff0bff2cff2c80ff8080808080ffff0bff2cff8080808080ffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff2effff04ff02ffff04ff09ff80808080ffff02ff2effff04ff02ffff04ff0dff8080808080ffff01ff0bff2cff058080ff0180ffff04ffff04ff28ffff04ff5fff808080ffff02ff7effff04ff02ffff04ffff04ffff04ff2fff0580ffff04ff5fff82017f8080ffff04ffff02ff7affff04ff02ffff04ff0bffff04ff05ffff01ff808080808080ffff04ff17ffff04ff81bfffff04ff82017fffff04ffff0bff8204ffffff02ff36ffff04ff02ffff04ff09ffff04ff820affffff04ffff0bff2cff2d80ffff04ff15ff80808080808080ff8216ff80ffff04ff8205ffffff04ff820bffff808080808080808080808080ff02ff2affff04ff02ffff04ff5fffff04ff3bffff04ffff02ffff03ff17ffff01ff09ff2dffff0bff27ffff02ff36ffff04ff02ffff04ff29ffff04ff57ffff04ffff0bff2cff81b980ffff04ff59ff80808080808080ff81b78080ff8080ff0180ffff04ff17ffff04ff05ffff04ff8202ffffff04ffff04ffff04ff24ffff04ffff0bff7cff2fff82017f80ff808080ffff04ffff04ff30ffff04ffff0bff81bfffff0bff7cff15ffff10ff82017fffff11ff8202dfff2b80ff8202ff808080ff808080ff138080ff80808080808080808080ff018080"  # noqa
 )
 
-OFFER_MOD_OLD = load_clvm_maybe_recompile("settlement_payments_old.clvm")
-OFFER_MOD = load_clvm_maybe_recompile("settlement_payments.clvm")
+OFFER_MOD_OLD = load_clvm_maybe_recompile("settlement_payments_old.clsp")
+OFFER_MOD = load_clvm_maybe_recompile("settlement_payments.clsp")
 
 # For backwards compatibility to work, we must assume that these mods (already deployed) will not change
 # In the case that they do change and we don't support the old asset then we need to keep around the legacy module
 ZDICT = [
     bytes(standard_puzzle.MOD) + bytes(LEGACY_CAT_MOD),
     bytes(OFFER_MOD_OLD),
     bytes(SINGLETON_TOP_LAYER_MOD)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/wallet_sync_utils.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/wallet_sync_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     RespondRemovals,
     RespondToCoinUpdates,
     RespondToPhUpdates,
 )
 from chia.server.ws_connection import WSChiaConnection
 from chia.types.blockchain_format.coin import Coin, hash_coin_ids
 from chia.types.blockchain_format.sized_bytes import bytes32
+from chia.types.coin_spend import CoinSpend
 from chia.types.full_block import FullBlock
 from chia.types.header_block import HeaderBlock
 from chia.util.ints import uint32
 from chia.util.merkle_set import MerkleSet, confirm_included_already_hashed, confirm_not_included_already_hashed
 from chia.wallet.util.peer_request_cache import PeerRequestCache
 
 log = logging.getLogger(__name__)
@@ -404,7 +405,29 @@
             peer_request_cache.add_to_block_requests(request_start, request_end, res_h_blocks_task)
             res_h_blocks = await res_h_blocks_task
         if res_h_blocks is None:
             return None
         assert res_h_blocks is not None
         blocks.extend([bl for bl in res_h_blocks.header_blocks if bl.height >= start])
     return blocks
+
+
+async def fetch_coin_spend(height: uint32, coin: Coin, peer: WSChiaConnection) -> CoinSpend:
+    solution_response = await peer.call_api(
+        FullNodeAPI.request_puzzle_solution, wallet_protocol.RequestPuzzleSolution(coin.name(), height)
+    )
+    if solution_response is None or not isinstance(solution_response, wallet_protocol.RespondPuzzleSolution):
+        raise PeerRequestException(f"Was not able to obtain solution {solution_response}")
+    assert solution_response.response.puzzle.get_tree_hash() == coin.puzzle_hash
+    assert solution_response.response.coin_name == coin.name()
+
+    return CoinSpend(
+        coin,
+        solution_response.response.puzzle,
+        solution_response.response.solution,
+    )
+
+
+async def fetch_coin_spend_for_coin_state(coin_state: CoinState, peer: WSChiaConnection) -> CoinSpend:
+    if coin_state.spent_height is None:
+        raise ValueError("coin_state.coin must be spent coin")
+    return await fetch_coin_spend(uint32(coin_state.spent_height), coin_state.coin, peer)
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/util/wallet_types.py` & `chia-blockchain-1.8.0rc1/chia/wallet/util/wallet_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_action.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_action.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_blockchain.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_coin_record.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_coin_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_coin_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_info.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_interested_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_interested_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_nft_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_nft_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_node.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from chia.server.node_discovery import WalletPeers
 from chia.server.outbound_message import Message, NodeType, make_msg
 from chia.server.peer_store_resolver import PeerStoreResolver
 from chia.server.server import ChiaServer
 from chia.server.ws_connection import WSChiaConnection
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.sized_bytes import bytes32
-from chia.types.coin_spend import CoinSpend
 from chia.types.header_block import HeaderBlock
 from chia.types.mempool_inclusion_status import MempoolInclusionStatus
 from chia.types.spend_bundle import SpendBundle
 from chia.types.weight_proof import WeightProof
 from chia.util.chunks import chunks
 from chia.util.config import (
     WALLET_PEERS_PATH_KEY_DEPRECATED,
@@ -1552,29 +1551,14 @@
             return False
         for header_block in sigs_to_cache:
             peer_request_cache.add_to_block_signatures_validated(header_block)
         for reward_chain_hash, height in blocks_to_cache:
             peer_request_cache.add_to_blocks_validated(reward_chain_hash, height)
         return True
 
-    async def fetch_puzzle_solution(self, height: uint32, coin: Coin, peer: WSChiaConnection) -> CoinSpend:
-        solution_response = await peer.call_api(
-            FullNodeAPI.request_puzzle_solution, wallet_protocol.RequestPuzzleSolution(coin.name(), height)
-        )
-        if solution_response is None or not isinstance(solution_response, wallet_protocol.RespondPuzzleSolution):
-            raise PeerRequestException(f"Was not able to obtain solution {solution_response}")
-        assert solution_response.response.puzzle.get_tree_hash() == coin.puzzle_hash
-        assert solution_response.response.coin_name == coin.name()
-
-        return CoinSpend(
-            coin,
-            solution_response.response.puzzle,
-            solution_response.response.solution,
-        )
-
     async def get_coin_state(
         self, coin_names: List[bytes32], peer: WSChiaConnection, fork_height: Optional[uint32] = None
     ) -> List[CoinState]:
         msg = wallet_protocol.RegisterForCoinUpdates(coin_names, uint32(0))
         coin_state: Optional[RespondToCoinUpdates] = await peer.call_api(FullNodeAPI.register_interest_in_coin, msg)
         if coin_state is None or not isinstance(coin_state, wallet_protocol.RespondToCoinUpdates):
             raise PeerRequestException(f"Was not able to get states for {coin_names}")
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_node_api.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_node_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_pool_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_pool_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_protocol.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_puzzle_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_puzzle_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_retry_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_retry_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_state_manager.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_state_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,19 @@
 from chia.wallet.trade_manager import TradeManager
 from chia.wallet.trading.trade_status import TradeStatus
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 from chia.wallet.util.address_type import AddressType
 from chia.wallet.util.compute_hints import compute_coin_hints
 from chia.wallet.util.transaction_type import TransactionType
-from chia.wallet.util.wallet_sync_utils import PeerRequestException, last_change_height_cs
+from chia.wallet.util.wallet_sync_utils import (
+    PeerRequestException,
+    fetch_coin_spend_for_coin_state,
+    last_change_height_cs,
+)
 from chia.wallet.util.wallet_types import WalletIdentifier, WalletType
 from chia.wallet.wallet import Wallet
 from chia.wallet.wallet_blockchain import WalletBlockchain
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_coin_store import WalletCoinStore
 from chia.wallet.wallet_info import WalletInfo
 from chia.wallet.wallet_interested_store import WalletInterestedStore
@@ -617,17 +621,15 @@
         )
         if len(response) == 0:
             self.log.warning(f"Could not find a parent coin with ID: {coin_state.coin.parent_coin_info}")
             return None
         parent_coin_state = response[0]
         assert parent_coin_state.spent_height == coin_state.created_height
 
-        coin_spend: Optional[CoinSpend] = await self.wallet_node.fetch_puzzle_solution(
-            parent_coin_state.spent_height, parent_coin_state.coin, peer
-        )
+        coin_spend = await fetch_coin_spend_for_coin_state(parent_coin_state, peer)
         if coin_spend is None:
             return None
 
         puzzle = Program.from_bytes(bytes(coin_spend.puzzle_reveal))
 
         uncurried = uncurry_puzzle(puzzle)
 
@@ -829,17 +831,15 @@
             wallet_identifier = WalletIdentifier.create(did_wallet)
             self.state_changed("wallet_created", wallet_identifier.id, {"did_id": did_wallet.get_my_DID()})
             return wallet_identifier
 
     async def get_minter_did(self, launcher_coin: Coin, peer: WSChiaConnection) -> Optional[bytes32]:
         # Get minter DID
         eve_coin = (await self.wallet_node.fetch_children(launcher_coin.name(), peer=peer))[0]
-        eve_coin_spend: CoinSpend = await self.wallet_node.fetch_puzzle_solution(
-            eve_coin.spent_height, eve_coin.coin, peer
-        )
+        eve_coin_spend = await fetch_coin_spend_for_coin_state(eve_coin, peer)
         eve_full_puzzle: Program = Program.from_bytes(bytes(eve_coin_spend.puzzle_reveal))
         eve_uncurried_nft: Optional[UncurriedNFT] = UncurriedNFT.uncurry(*eve_full_puzzle.uncurry())
         if eve_uncurried_nft is None:
             raise ValueError("Couldn't get minter DID for NFT")
         if not eve_uncurried_nft.supports_did:
             return None
         minter_did = get_new_owner_did(eve_uncurried_nft, eve_coin_spend.solution.to_program())
@@ -855,17 +855,15 @@
                 and len(launcher_parent) == 1
                 and launcher_parent[0].spent_height is not None
             )
             did_coin: List[CoinState] = await self.wallet_node.get_coin_state(
                 [launcher_parent[0].coin.parent_coin_info], peer=peer
             )
             assert did_coin is not None and len(did_coin) == 1 and did_coin[0].spent_height is not None
-            did_spend: CoinSpend = await self.wallet_node.fetch_puzzle_solution(
-                did_coin[0].spent_height, did_coin[0].coin, peer
-            )
+            did_spend = await fetch_coin_spend_for_coin_state(did_coin[0], peer)
             puzzle = Program.from_bytes(bytes(did_spend.puzzle_reveal))
             uncurried = uncurry_puzzle(puzzle)
             did_curried_args = match_did_puzzle(uncurried.mod, uncurried.args)
             if did_curried_args is not None:
                 p2_puzzle, recovery_list_hash, num_verification, singleton_struct, metadata = did_curried_args
                 minter_did = bytes32(bytes(singleton_struct.rest().first())[1:])
         return minter_did
@@ -1206,17 +1204,15 @@
 
                         if record.wallet_type == WalletType.POOLING_WALLET:
                             if coin_state.spent_height is not None and coin_state.coin.amount == uint64(1):
                                 pool_wallet = self.get_wallet(id=uint32(record.wallet_id), required_type=PoolWallet)
                                 curr_coin_state: CoinState = coin_state
 
                                 while curr_coin_state.spent_height is not None:
-                                    cs: CoinSpend = await self.wallet_node.fetch_puzzle_solution(
-                                        curr_coin_state.spent_height, curr_coin_state.coin, peer
-                                    )
+                                    cs = await fetch_coin_spend_for_coin_state(curr_coin_state, peer)
                                     success = await pool_wallet.apply_state_transition(
                                         cs, uint32(curr_coin_state.spent_height)
                                     )
                                     if not success:
                                         break
                                     new_singleton_coin: Optional[Coin] = pool_wallet.get_next_interesting_coin(cs)
                                     if new_singleton_coin is None:
@@ -1241,17 +1237,15 @@
                                     await self.add_interested_coin_ids([new_singleton_coin.name()])
                                     new_coin_state: List[CoinState] = await self.wallet_node.get_coin_state(
                                         [coin_name], peer=peer, fork_height=fork_height
                                     )
                                     assert len(new_coin_state) == 1
                                     curr_coin_state = new_coin_state[0]
                         if record.wallet_type == WalletType.DATA_LAYER:
-                            singleton_spend = await self.wallet_node.fetch_puzzle_solution(
-                                coin_state.spent_height, coin_state.coin, peer
-                            )
+                            singleton_spend = await fetch_coin_spend_for_coin_state(coin_state, peer)
                             dl_wallet = self.get_wallet(id=uint32(record.wallet_id), required_type=DataLayerWallet)
                             await dl_wallet.singleton_removed(
                                 singleton_spend,
                                 uint32(coin_state.spent_height),
                             )
 
                         elif record.wallet_type == WalletType.NFT:
@@ -1264,17 +1258,15 @@
                             if child.coin.puzzle_hash != SINGLETON_LAUNCHER_HASH:
                                 continue
                             if await self.have_a_pool_wallet_with_launched_id(child.coin.name()):
                                 continue
                             if child.spent_height is None:
                                 # TODO handle spending launcher later block
                                 continue
-                            launcher_spend: Optional[CoinSpend] = await self.wallet_node.fetch_puzzle_solution(
-                                child.spent_height, child.coin, peer
-                            )
+                            launcher_spend = await fetch_coin_spend_for_coin_state(child, peer)
                             if launcher_spend is None:
                                 continue
                             try:
                                 pool_state = solution_to_pool_state(launcher_spend)
                                 assert pool_state is not None
                             except (AssertionError, ValueError) as e:
                                 self.log.debug(f"Not a pool wallet launcher {e}, child: {child}")
```

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_transaction_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_transaction_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_user_store.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_user_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia/wallet/wallet_weight_proof_handler.py` & `chia-blockchain-1.8.0rc1/chia/wallet/wallet_weight_proof_handler.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/PKG-INFO` & `chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia-blockchain
-Version: 1.8.0b6
+Version: 1.8.0rc1
 Summary: Chia blockchain full node, farmer, timelord, and wallet.
 Home-page: https://chia.net/
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Project-URL: Source, https://github.com/Chia-Network/chia-blockchain/
 Project-URL: Changelog, https://github.com/Chia-Network/chia-blockchain/blob/main/CHANGELOG.md
```

### Comparing `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/SOURCES.txt` & `chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 .github/workflows/build-linux-installer-rpm.yml
 .github/workflows/build-macos-installers.yml
 .github/workflows/build-windows-installer.yml
 .github/workflows/check-commit-signing.yml
 .github/workflows/check_wheel_availability.yaml
 .github/workflows/codeql-analysis.yml
 .github/workflows/conflict-check.yml
+.github/workflows/daily-matrix.yml
 .github/workflows/dependency-review.yml
 .github/workflows/mozilla-ca-cert.yml
 .github/workflows/pre-commit.yml
 .github/workflows/require-labels.yml
 .github/workflows/snyk-python-scan.yml
 .github/workflows/stale-issue.yml
 .github/workflows/start-release.yml
@@ -129,14 +130,15 @@
 chia/cmds/configure.py
 chia/cmds/data.py
 chia/cmds/data_funcs.py
 chia/cmds/db.py
 chia/cmds/db_backup_func.py
 chia/cmds/db_upgrade_func.py
 chia/cmds/db_validate_func.py
+chia/cmds/dev.py
 chia/cmds/farm.py
 chia/cmds/farm_funcs.py
 chia/cmds/init.py
 chia/cmds/init_funcs.py
 chia/cmds/keys.py
 chia/cmds/keys_funcs.py
 chia/cmds/netspace.py
@@ -148,14 +150,16 @@
 chia/cmds/plotnft.py
 chia/cmds/plotnft_funcs.py
 chia/cmds/plots.py
 chia/cmds/plotters.py
 chia/cmds/rpc.py
 chia/cmds/show.py
 chia/cmds/show_funcs.py
+chia/cmds/sim.py
+chia/cmds/sim_funcs.py
 chia/cmds/start.py
 chia/cmds/start_funcs.py
 chia/cmds/stop.py
 chia/cmds/units.py
 chia/cmds/wallet.py
 chia/cmds/wallet_funcs.py
 chia/consensus/__init__.py
@@ -524,163 +528,119 @@
 chia/wallet/nft_wallet/nft_puzzles.py
 chia/wallet/nft_wallet/nft_wallet.py
 chia/wallet/nft_wallet/ownership_outer_puzzle.py
 chia/wallet/nft_wallet/singleton_outer_puzzle.py
 chia/wallet/nft_wallet/transfer_program_puzzle.py
 chia/wallet/nft_wallet/uncurry_nft.py
 chia/wallet/puzzles/__init__.py
-chia/wallet/puzzles/block_program_zero.clvm
-chia/wallet/puzzles/block_program_zero.clvm.hex
-chia/wallet/puzzles/block_program_zero.clvm.hex.sha256tree
-chia/wallet/puzzles/calculate_synthetic_public_key.clvm
-chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex
-chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex.sha256tree
+chia/wallet/puzzles/block_program_zero.clsp
+chia/wallet/puzzles/block_program_zero.clsp.hex
+chia/wallet/puzzles/calculate_synthetic_public_key.clsp
+chia/wallet/puzzles/calculate_synthetic_public_key.clsp.hex
 chia/wallet/puzzles/cat_loader.py
 chia/wallet/puzzles/cat_truths.clib
-chia/wallet/puzzles/cat_v2.clvm
-chia/wallet/puzzles/cat_v2.clvm.hex
-chia/wallet/puzzles/cat_v2.clvm.hex.sha256tree
-chia/wallet/puzzles/chialisp_deserialisation.clvm
-chia/wallet/puzzles/chialisp_deserialisation.clvm.hex
-chia/wallet/puzzles/chialisp_deserialisation.clvm.hex.sha256tree
-chia/wallet/puzzles/condition_codes.clvm
-chia/wallet/puzzles/create-lock-puzzlehash.clvm
-chia/wallet/puzzles/create_nft_launcher_from_did.clvm
-chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex
-chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex.sha256tree
-chia/wallet/puzzles/curry-and-treehash.clinc
+chia/wallet/puzzles/cat_v2.clsp
+chia/wallet/puzzles/cat_v2.clsp.hex
+chia/wallet/puzzles/chialisp_deserialisation.clsp
+chia/wallet/puzzles/chialisp_deserialisation.clsp.hex
+chia/wallet/puzzles/condition_codes.clib
+chia/wallet/puzzles/create-lock-puzzlehash.clib
+chia/wallet/puzzles/create_nft_launcher_from_did.clsp
+chia/wallet/puzzles/create_nft_launcher_from_did.clsp.hex
+chia/wallet/puzzles/curry-and-treehash.clib
 chia/wallet/puzzles/curry.clib
-chia/wallet/puzzles/decompress_coin_spend_entry.clvm
-chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex
-chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex.sha256tree
-chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm
-chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex
-chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex.sha256tree
-chia/wallet/puzzles/decompress_puzzle.clvm
-chia/wallet/puzzles/decompress_puzzle.clvm.hex
-chia/wallet/puzzles/decompress_puzzle.clvm.hex.sha256tree
-chia/wallet/puzzles/delegated_tail.clvm
-chia/wallet/puzzles/delegated_tail.clvm.hex
-chia/wallet/puzzles/delegated_tail.clvm.hex.sha256tree
-chia/wallet/puzzles/did_innerpuz.clvm
-chia/wallet/puzzles/did_innerpuz.clvm.hex
-chia/wallet/puzzles/did_innerpuz.clvm.hex.sha256tree
-chia/wallet/puzzles/everything_with_signature.clvm
-chia/wallet/puzzles/everything_with_signature.clvm.hex
-chia/wallet/puzzles/everything_with_signature.clvm.hex.sha256tree
-chia/wallet/puzzles/genesis_by_coin_id.clvm
-chia/wallet/puzzles/genesis_by_coin_id.clvm.hex
-chia/wallet/puzzles/genesis_by_coin_id.clvm.hex.sha256tree
-chia/wallet/puzzles/genesis_by_puzzle_hash.clvm
-chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex
-chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex.sha256tree
-chia/wallet/puzzles/graftroot_dl_offers.clvm
-chia/wallet/puzzles/graftroot_dl_offers.clvm.hex
-chia/wallet/puzzles/graftroot_dl_offers.clvm.hex.sha256tree
+chia/wallet/puzzles/decompress_coin_spend_entry.clsp
+chia/wallet/puzzles/decompress_coin_spend_entry.clsp.hex
+chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clsp
+chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clsp.hex
+chia/wallet/puzzles/decompress_puzzle.clsp
+chia/wallet/puzzles/decompress_puzzle.clsp.hex
+chia/wallet/puzzles/delegated_tail.clsp
+chia/wallet/puzzles/delegated_tail.clsp.hex
+chia/wallet/puzzles/deployed_puzzle_hashes.json
+chia/wallet/puzzles/did_innerpuz.clsp
+chia/wallet/puzzles/did_innerpuz.clsp.hex
+chia/wallet/puzzles/everything_with_signature.clsp
+chia/wallet/puzzles/everything_with_signature.clsp.hex
+chia/wallet/puzzles/genesis_by_coin_id.clsp
+chia/wallet/puzzles/genesis_by_coin_id.clsp.hex
+chia/wallet/puzzles/genesis_by_puzzle_hash.clsp
+chia/wallet/puzzles/genesis_by_puzzle_hash.clsp.hex
+chia/wallet/puzzles/graftroot_dl_offers.clsp
+chia/wallet/puzzles/graftroot_dl_offers.clsp.hex
 chia/wallet/puzzles/json.clib
 chia/wallet/puzzles/load_clvm.py
-chia/wallet/puzzles/lock.inner.puzzle.clvm
-chia/wallet/puzzles/lock.inner.puzzle.clvm.hex
-chia/wallet/puzzles/lock.inner.puzzle.clvm.hex.sha256tree
 chia/wallet/puzzles/merkle_utils.clib
-chia/wallet/puzzles/nft_intermediate_launcher.clvm
-chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex
-chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex.sha256tree
-chia/wallet/puzzles/nft_metadata_updater_default.clvm
-chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex
-chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex.sha256tree
-chia/wallet/puzzles/nft_metadata_updater_updateable.clvm
-chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex
-chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex.sha256tree
-chia/wallet/puzzles/nft_ownership_layer.clvm
-chia/wallet/puzzles/nft_ownership_layer.clvm.hex
-chia/wallet/puzzles/nft_ownership_layer.clvm.hex.sha256tree
-chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm
-chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex
-chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex.sha256tree
-chia/wallet/puzzles/nft_state_layer.clvm
-chia/wallet/puzzles/nft_state_layer.clvm.hex
-chia/wallet/puzzles/nft_state_layer.clvm.hex.sha256tree
-chia/wallet/puzzles/notification.clvm
-chia/wallet/puzzles/notification.clvm.hex
-chia/wallet/puzzles/notification.clvm.hex.sha256tree
-chia/wallet/puzzles/p2_conditions.clvm
-chia/wallet/puzzles/p2_conditions.clvm.hex
-chia/wallet/puzzles/p2_conditions.clvm.hex.sha256tree
+chia/wallet/puzzles/nft_intermediate_launcher.clsp
+chia/wallet/puzzles/nft_intermediate_launcher.clsp.hex
+chia/wallet/puzzles/nft_metadata_updater_default.clsp
+chia/wallet/puzzles/nft_metadata_updater_default.clsp.hex
+chia/wallet/puzzles/nft_metadata_updater_updateable.clsp
+chia/wallet/puzzles/nft_metadata_updater_updateable.clsp.hex
+chia/wallet/puzzles/nft_ownership_layer.clsp
+chia/wallet/puzzles/nft_ownership_layer.clsp.hex
+chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clsp
+chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clsp.hex
+chia/wallet/puzzles/nft_state_layer.clsp
+chia/wallet/puzzles/nft_state_layer.clsp.hex
+chia/wallet/puzzles/notification.clsp
+chia/wallet/puzzles/notification.clsp.hex
+chia/wallet/puzzles/p2_conditions.clsp
+chia/wallet/puzzles/p2_conditions.clsp.hex
 chia/wallet/puzzles/p2_conditions.py
-chia/wallet/puzzles/p2_delegated_conditions.clvm
-chia/wallet/puzzles/p2_delegated_conditions.clvm.hex
-chia/wallet/puzzles/p2_delegated_conditions.clvm.hex.sha256tree
+chia/wallet/puzzles/p2_delegated_conditions.clsp
+chia/wallet/puzzles/p2_delegated_conditions.clsp.hex
 chia/wallet/puzzles/p2_delegated_conditions.py
-chia/wallet/puzzles/p2_delegated_puzzle.clvm
-chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex
-chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex.sha256tree
+chia/wallet/puzzles/p2_delegated_puzzle.clsp
+chia/wallet/puzzles/p2_delegated_puzzle.clsp.hex
 chia/wallet/puzzles/p2_delegated_puzzle.py
-chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm
-chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex
-chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex.sha256tree
+chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clsp
+chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clsp.hex
 chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py
-chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm
-chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex
-chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex.sha256tree
+chia/wallet/puzzles/p2_m_of_n_delegate_direct.clsp
+chia/wallet/puzzles/p2_m_of_n_delegate_direct.clsp.hex
 chia/wallet/puzzles/p2_m_of_n_delegate_direct.py
-chia/wallet/puzzles/p2_parent.clvm
-chia/wallet/puzzles/p2_parent.clvm.hex
-chia/wallet/puzzles/p2_parent.clvm.hex.sha256tree
-chia/wallet/puzzles/p2_puzzle_hash.clvm
-chia/wallet/puzzles/p2_puzzle_hash.clvm.hex
-chia/wallet/puzzles/p2_puzzle_hash.clvm.hex.sha256tree
+chia/wallet/puzzles/p2_parent.clsp
+chia/wallet/puzzles/p2_parent.clsp.hex
+chia/wallet/puzzles/p2_puzzle_hash.clsp
+chia/wallet/puzzles/p2_puzzle_hash.clsp.hex
 chia/wallet/puzzles/p2_puzzle_hash.py
-chia/wallet/puzzles/p2_singleton.clvm
-chia/wallet/puzzles/p2_singleton.clvm.hex
-chia/wallet/puzzles/p2_singleton.clvm.hex.sha256tree
-chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm
-chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex
-chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex.sha256tree
-chia/wallet/puzzles/pool_member_innerpuz.clvm
-chia/wallet/puzzles/pool_member_innerpuz.clvm.hex
-chia/wallet/puzzles/pool_member_innerpuz.clvm.hex.sha256tree
-chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm
-chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex
-chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex.sha256tree
+chia/wallet/puzzles/p2_singleton.clsp
+chia/wallet/puzzles/p2_singleton.clsp.hex
+chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clsp
+chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clsp.hex
+chia/wallet/puzzles/pool_member_innerpuz.clsp
+chia/wallet/puzzles/pool_member_innerpuz.clsp.hex
+chia/wallet/puzzles/pool_waitingroom_innerpuz.clsp
+chia/wallet/puzzles/pool_waitingroom_innerpuz.clsp.hex
 chia/wallet/puzzles/puzzle_utils.py
-chia/wallet/puzzles/recompile-all.sh
-chia/wallet/puzzles/rom_bootstrap_generator.clvm
-chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex
-chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex.sha256tree
+chia/wallet/puzzles/rom_bootstrap_generator.clsp
+chia/wallet/puzzles/rom_bootstrap_generator.clsp.hex
 chia/wallet/puzzles/rom_bootstrap_generator.py
-chia/wallet/puzzles/settlement_payments.clvm
-chia/wallet/puzzles/settlement_payments.clvm.hex
-chia/wallet/puzzles/settlement_payments.clvm.hex.sha256tree
-chia/wallet/puzzles/settlement_payments_old.clvm
-chia/wallet/puzzles/settlement_payments_old.clvm.hex
-chia/wallet/puzzles/settlement_payments_old.clvm.hex.sha256tree
+chia/wallet/puzzles/settlement_payments.clsp
+chia/wallet/puzzles/settlement_payments.clsp.hex
+chia/wallet/puzzles/settlement_payments_old.clsp
+chia/wallet/puzzles/settlement_payments_old.clsp.hex
 chia/wallet/puzzles/sha256tree.clib
-chia/wallet/puzzles/sha256tree_module.clvm
-chia/wallet/puzzles/sha256tree_module.clvm.hex
-chia/wallet/puzzles/sha256tree_module.clvm.hex.sha256tree
-chia/wallet/puzzles/singleton_launcher.clvm
-chia/wallet/puzzles/singleton_launcher.clvm.hex
-chia/wallet/puzzles/singleton_launcher.clvm.hex.sha256tree
-chia/wallet/puzzles/singleton_top_layer.clvm
-chia/wallet/puzzles/singleton_top_layer.clvm.hex
-chia/wallet/puzzles/singleton_top_layer.clvm.hex.sha256tree
+chia/wallet/puzzles/sha256tree_module.clsp
+chia/wallet/puzzles/sha256tree_module.clsp.hex
+chia/wallet/puzzles/singleton_launcher.clsp
+chia/wallet/puzzles/singleton_launcher.clsp.hex
+chia/wallet/puzzles/singleton_top_layer.clsp
+chia/wallet/puzzles/singleton_top_layer.clsp.hex
 chia/wallet/puzzles/singleton_top_layer.py
-chia/wallet/puzzles/singleton_top_layer_v1_1.clvm
-chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex
-chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex.sha256tree
+chia/wallet/puzzles/singleton_top_layer_v1_1.clsp
+chia/wallet/puzzles/singleton_top_layer_v1_1.clsp.hex
 chia/wallet/puzzles/singleton_top_layer_v1_1.py
 chia/wallet/puzzles/singleton_truths.clib
 chia/wallet/puzzles/tails.py
-chia/wallet/puzzles/test_generator_deserialize.clvm
-chia/wallet/puzzles/test_generator_deserialize.clvm.hex
-chia/wallet/puzzles/test_generator_deserialize.clvm.hex.sha256tree
-chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm
-chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex
-chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex.sha256tree
+chia/wallet/puzzles/test_generator_deserialize.clsp
+chia/wallet/puzzles/test_generator_deserialize.clsp.hex
+chia/wallet/puzzles/test_multiple_generator_input_arguments.clsp
+chia/wallet/puzzles/test_multiple_generator_input_arguments.clsp.hex
 chia/wallet/puzzles/utility_macros.clib
 chia/wallet/puzzles/prefarm/__init__.py
 chia/wallet/puzzles/prefarm/make_prefarm_ph.py
 chia/wallet/puzzles/prefarm/spend_prefarm.py
 chia/wallet/trading/__init__.py
 chia/wallet/trading/offer.py
 chia/wallet/trading/trade_status.py
@@ -736,14 +696,15 @@
 tests/clvm/test_puzzle_compression.py
 tests/clvm/test_puzzle_drivers.py
 tests/clvm/test_puzzles.py
 tests/clvm/test_serialized_program.py
 tests/clvm/test_singletons.py
 tests/clvm/test_spend_sim.py
 tests/cmds/__init__.py
+tests/cmds/test_sim.py
 tests/cmds/test_wallet_check.py
 tests/core/__init__.py
 tests/core/config.py
 tests/core/large_block.py
 tests/core/make_block_generator.py
 tests/core/node_height.py
 tests/core/test_coins.py
```

### Comparing `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/entry_points.txt` & `chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/requires.txt` & `chia-blockchain-1.8.0rc1/chia_blockchain.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 boto3==1.26.111
 blspy==1.0.16
 chiavdf==1.0.8
 chiabip158==1.2
 chiapos==1.0.11
 clvm==0.9.7
 clvm_tools==0.4.6
-chia_rs==0.2.5
+chia_rs==0.2.6
 clvm-tools-rs==0.1.30
 aiohttp==3.8.4
 aiosqlite==0.17.0
 bitstring==4.0.1
 colorama==0.4.6
 colorlog==6.7.0
 concurrent-log-handler==0.9.20
```

### Comparing `chia-blockchain-1.8.0b6/install-gui.sh` & `chia-blockchain-1.8.0rc1/install-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/install-plotter.sh` & `chia-blockchain-1.8.0rc1/install-plotter.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/install-timelord.sh` & `chia-blockchain-1.8.0rc1/install-timelord.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/install.sh` & `chia-blockchain-1.8.0rc1/install.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/installhelper.py` & `chia-blockchain-1.8.0rc1/installhelper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/mozilla-ca/cacert.pem` & `chia-blockchain-1.8.0rc1/mozilla-ca/cacert.pem`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/mypy.ini` & `chia-blockchain-1.8.0rc1/mypy.ini`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 no_implicit_optional = True
 warn_return_any = True
 no_implicit_reexport = True
 strict_equality = True
 warn_redundant_casts = True
 
 # list created by: venv/bin/mypy | sed -n 's/.py:.*//p' | sort | uniq | tr '/' '.' | tr '\n' ','
-[mypy-chia.cmds.passphrase,chia.cmds.passphrase_funcs,chia.cmds.plots,chia.cmds.plotters,chia.cmds.show,chia.cmds.start_funcs,chia.cmds.wallet,chia.cmds.wallet_funcs,chia.daemon.server,chia.farmer.farmer_api,chia.full_node.weight_proof,chia.introducer.introducer,chia.introducer.introducer_api,chia.plotters.bladebit,chia.plotters.chiapos,chia.plotters.madmax,chia.plotters.plotters,chia.plotters.plotters_util,chia.plotting.create_plots,chia.plotting.manager,chia.plotting.util,chia.pools.pool_puzzles,chia.pools.pool_wallet,chia.pools.pool_wallet_info,chia.rpc.full_node_rpc_client,chia.rpc.harvester_rpc_api,chia.rpc.harvester_rpc_client,chia.rpc.rpc_client,chia.rpc.timelord_rpc_api,chia.rpc.util,chia.rpc.wallet_rpc_api,chia.rpc.wallet_rpc_client,chia.seeder.crawler,chia.seeder.crawler_api,chia.seeder.crawl_store,chia.seeder.dns_server,chia.seeder.peer_record,chia.seeder.start_crawler,chia.simulator.full_node_simulator,chia.simulator.start_simulator,chia.ssl.create_ssl,chia.timelord.iters_from_block,chia.timelord.timelord,chia.timelord.timelord_api,chia.timelord.timelord_launcher,chia.timelord.timelord_state,chia.types.blockchain_format.program,chia.util.block_cache,chia.util.check_fork_next_block,chia.util.chia_logging,chia.util.config,chia.util.db_wrapper,chia.util.dump_keyring,chia.util.hash,chia.util.json_util,chia.util.keychain,chia.util.keyring_wrapper,chia.util.log_exceptions,chia.util.make_test_constants,chia.util.merkle_set,chia.util.network,chia.util.partial_func,chia.util.profiler,chia.util.safe_cancel_task,chia.util.service_groups,chia.util.ssl_check,chia.util.validate_alert,chia.wallet.block_record,chia.wallet.chialisp,chia.wallet.did_wallet.did_wallet,chia.wallet.did_wallet.did_wallet_puzzles,chia.wallet.key_val_store,chia.wallet.lineage_proof,chia.wallet.payment,chia.wallet.puzzles.load_clvm,chia.wallet.puzzles.p2_conditions,chia.wallet.puzzles.p2_delegated_conditions,chia.wallet.puzzles.p2_delegated_puzzle,chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle,chia.wallet.puzzles.p2_m_of_n_delegate_direct,chia.wallet.puzzles.p2_puzzle_hash,chia.wallet.puzzles.prefarm.spend_prefarm,chia.wallet.puzzles.puzzle_utils,chia.wallet.puzzles.singleton_top_layer,chia.wallet.puzzles.tails,chia.wallet.secret_key_store,chia.wallet.trade_record,chia.wallet.trading.trade_store,chia.wallet.transaction_record,chia.wallet.util.debug_spend_bundle,chia.wallet.util.new_peak_queue,chia.wallet.wallet,chia.wallet.wallet_coin_store,chia.wallet.wallet_interested_store,chia.wallet.wallet_node_api,chia.wallet.wallet_pool_store,chia.wallet.wallet_puzzle_store,chia.wallet.wallet_state_manager,chia.wallet.wallet_sync_store,chia.wallet.wallet_transaction_store,chia.wallet.wallet_user_store,installhelper,tests.blockchain.blockchain_test_utils,tests.blockchain.test_blockchain,tests.blockchain.test_blockchain_transactions,chia.simulator.block_tools,tests.build-init-files,tests.build-workflows,tests.clvm.coin_store,tests.clvm.test_chialisp_deserialization,tests.clvm.test_clvm_compilation,tests.clvm.test_program,tests.clvm.test_puzzle_compression,tests.clvm.test_puzzles,tests.clvm.test_serialized_program,tests.clvm.test_singletons,tests.clvm.test_spend_sim,tests.conftest,tests.connection_utils,tests.core.cmds.test_keys,tests.core.consensus.test_pot_iterations,tests.core.custom_types.test_coin,tests.core.custom_types.test_proof_of_space,tests.core.custom_types.test_spend_bundle,tests.core.daemon.test_daemon,tests.core.full_node.full_sync.test_full_sync,tests.core.full_node.stores.test_block_store,tests.core.full_node.stores.test_coin_store,tests.core.full_node.stores.test_full_node_store,tests.core.full_node.stores.test_hint_store,tests.core.full_node.stores.test_sync_store,tests.core.full_node.test_address_manager,tests.core.full_node.test_block_height_map,tests.core.full_node.test_conditions,tests.core.full_node.test_full_node,tests.core.mempool.test_mempool,tests.core.mempool.test_mempool_performance,tests.core.full_node.test_node_load,tests.core.full_node.test_peer_store_resolver,tests.core.full_node.test_performance,tests.core.full_node.test_transactions,tests.core.make_block_generator,tests.core.node_height,tests.core.server.test_dos,tests.core.server.test_rate_limits,tests.core.ssl.test_ssl,tests.core.test_cost_calculation,tests.core.test_crawler_rpc,tests.core.test_daemon_rpc,tests.core.test_db_conversion,tests.core.test_db_validation,tests.core.test_farmer_harvester_rpc,tests.core.test_filter,tests.core.test_full_node_rpc,tests.core.test_merkle_set,tests.core.test_setproctitle,tests.core.util.test_cached_bls,tests.core.util.test_config,tests.core.util.test_file_keyring_synchronization,tests.core.util.test_files,tests.core.util.test_keychain,tests.core.util.test_keyring_wrapper,tests.core.util.test_lru_cache,tests.core.util.test_significant_bits,tests.farmer_harvester.test_farmer_harvester,tests.generator.test_compression,tests.generator.test_generator_types,tests.generator.test_list_to_batches,tests.generator.test_rom,tests.generator.test_scan,tests.plotting.test_plot_manager,tests.pools.test_pool_cmdline,tests.pools.test_pool_config,tests.pools.test_pool_puzzles_lifecycle,tests.pools.test_wallet_pool_store,tests.simulation.test_simulation,chia.simulator.time_out_assert,tests.tools.test_full_sync,tests.tools.test_run_block,tests.util.alert_server,tests.util.benchmark_cost,tests.util.blockchain,tests.util.build_network_protocol_files,tests.util.db_connection,tests.util.generator_tools_testing,chia.simulator.keyring,tests.util.key_tool,tests.util.test_full_block_utils,tests.util.test_lock_queue,tests.util.test_misc,tests.util.test_network,tests.util.test_network_protocol_files,tests.wallet.cat_wallet.test_cat_lifecycle,tests.wallet.cat_wallet.test_cat_wallet,tests.wallet.cat_wallet.test_offer_lifecycle,tests.wallet.cat_wallet.test_trades,tests.wallet.did_wallet.test_did,tests.wallet.did_wallet.test_did_rpc,tests.wallet.did_wallet.test_nft_rpc,tests.wallet.did_wallet.test_nft_wallet,tests.wallet.rpc.test_wallet_rpc,tests.wallet.simple_sync.test_simple_sync_protocol,tests.wallet.sync.test_wallet_sync,tests.wallet.test_bech32m,tests.wallet.test_chialisp,tests.wallet.test_puzzle_store,tests.wallet.test_singleton,tests.wallet.test_singleton_lifecycle,tests.wallet.test_singleton_lifecycle_fast,tests.wallet.test_taproot,tests.wallet.test_wallet_blockchain,tests.wallet.test_wallet_interested_store,tests.wallet.test_wallet_key_val_store,tests.wallet.test_wallet_user_store,chia.simulator.wallet_tools,tests.weight_proof.test_weight_proof,tools.analyze-chain,tools.run_block,tools.test_full_sync,tests.wallet.nft_wallet.test_nft_wallet,chia.wallet.nft_wallet.nft_puzzles,tests.wallet.nft_wallet.test_nft_puzzles]
+[mypy-chia.cmds.passphrase,chia.cmds.passphrase_funcs,chia.cmds.plots,chia.cmds.plotters,chia.cmds.show,chia.cmds.start_funcs,chia.cmds.wallet,chia.cmds.wallet_funcs,chia.daemon.server,chia.farmer.farmer_api,chia.full_node.weight_proof,chia.introducer.introducer,chia.introducer.introducer_api,chia.plotters.bladebit,chia.plotters.chiapos,chia.plotters.madmax,chia.plotters.plotters,chia.plotters.plotters_util,chia.plotting.create_plots,chia.plotting.manager,chia.plotting.util,chia.pools.pool_puzzles,chia.pools.pool_wallet,chia.pools.pool_wallet_info,chia.rpc.full_node_rpc_client,chia.rpc.harvester_rpc_api,chia.rpc.harvester_rpc_client,chia.rpc.rpc_client,chia.rpc.timelord_rpc_api,chia.rpc.util,chia.rpc.wallet_rpc_api,chia.rpc.wallet_rpc_client,chia.seeder.crawler,chia.seeder.crawler_api,chia.seeder.crawl_store,chia.seeder.dns_server,chia.seeder.peer_record,chia.seeder.start_crawler,chia.simulator.full_node_simulator,chia.simulator.start_simulator,chia.ssl.create_ssl,chia.timelord.iters_from_block,chia.timelord.timelord,chia.timelord.timelord_api,chia.timelord.timelord_launcher,chia.timelord.timelord_state,chia.types.blockchain_format.program,chia.util.block_cache,chia.util.check_fork_next_block,chia.util.chia_logging,chia.util.config,chia.util.db_wrapper,chia.util.dump_keyring,chia.util.hash,chia.util.json_util,chia.util.keychain,chia.util.keyring_wrapper,chia.util.log_exceptions,chia.util.make_test_constants,chia.util.merkle_set,chia.util.network,chia.util.partial_func,chia.util.profiler,chia.util.safe_cancel_task,chia.util.service_groups,chia.util.ssl_check,chia.util.validate_alert,chia.wallet.block_record,chia.wallet.chialisp,chia.wallet.did_wallet.did_wallet,chia.wallet.did_wallet.did_wallet_puzzles,chia.wallet.key_val_store,chia.wallet.lineage_proof,chia.wallet.payment,chia.wallet.puzzles.load_clvm,chia.wallet.puzzles.p2_conditions,chia.wallet.puzzles.p2_delegated_conditions,chia.wallet.puzzles.p2_delegated_puzzle,chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle,chia.wallet.puzzles.p2_m_of_n_delegate_direct,chia.wallet.puzzles.p2_puzzle_hash,chia.wallet.puzzles.prefarm.spend_prefarm,chia.wallet.puzzles.puzzle_utils,chia.wallet.puzzles.singleton_top_layer,chia.wallet.puzzles.tails,chia.wallet.secret_key_store,chia.wallet.trade_record,chia.wallet.trading.trade_store,chia.wallet.transaction_record,chia.wallet.util.debug_spend_bundle,chia.wallet.util.new_peak_queue,chia.wallet.wallet,chia.wallet.wallet_coin_store,chia.wallet.wallet_interested_store,chia.wallet.wallet_node_api,chia.wallet.wallet_pool_store,chia.wallet.wallet_puzzle_store,chia.wallet.wallet_state_manager,chia.wallet.wallet_sync_store,chia.wallet.wallet_transaction_store,chia.wallet.wallet_user_store,installhelper,tests.blockchain.blockchain_test_utils,tests.blockchain.test_blockchain,tests.blockchain.test_blockchain_transactions,chia.simulator.block_tools,tests.build-init-files,tests.build-workflows,tests.clvm.coin_store,tests.clvm.test_chialisp_deserialization,tests.clvm.test_clvm_compilation,tests.clvm.test_program,tests.clvm.test_puzzle_compression,tests.clvm.test_puzzles,tests.clvm.test_serialized_program,tests.clvm.test_singletons,tests.clvm.test_spend_sim,tests.conftest,tests.connection_utils,tests.core.cmds.test_keys,tests.core.consensus.test_pot_iterations,tests.core.custom_types.test_coin,tests.core.custom_types.test_proof_of_space,tests.core.custom_types.test_spend_bundle,tests.core.daemon.test_daemon,tests.core.full_node.full_sync.test_full_sync,tests.core.full_node.stores.test_block_store,tests.core.full_node.stores.test_coin_store,tests.core.full_node.stores.test_full_node_store,tests.core.full_node.stores.test_hint_store,tests.core.full_node.stores.test_sync_store,tests.core.full_node.test_address_manager,tests.core.full_node.test_block_height_map,tests.core.full_node.test_conditions,tests.core.full_node.test_full_node,tests.core.mempool.test_mempool,tests.core.mempool.test_mempool_performance,tests.core.full_node.test_node_load,tests.core.full_node.test_peer_store_resolver,tests.core.full_node.test_performance,tests.core.full_node.test_transactions,tests.core.make_block_generator,tests.core.node_height,tests.core.server.test_dos,tests.core.server.test_rate_limits,tests.core.ssl.test_ssl,tests.core.test_cost_calculation,tests.core.test_crawler_rpc,tests.core.test_daemon_rpc,tests.core.test_db_conversion,tests.core.test_db_validation,tests.core.test_farmer_harvester_rpc,tests.core.test_filter,tests.core.test_full_node_rpc,tests.core.test_merkle_set,tests.core.test_setproctitle,tests.core.util.test_cached_bls,tests.core.util.test_config,tests.core.util.test_file_keyring_synchronization,tests.core.util.test_files,tests.core.util.test_keychain,tests.core.util.test_keyring_wrapper,tests.core.util.test_lru_cache,tests.core.util.test_significant_bits,tests.farmer_harvester.test_farmer_harvester,tests.generator.test_list_to_batches,tests.generator.test_scan,tests.plotting.test_plot_manager,tests.pools.test_pool_cmdline,tests.pools.test_pool_config,tests.pools.test_pool_puzzles_lifecycle,tests.pools.test_wallet_pool_store,tests.simulation.test_simulation,chia.simulator.time_out_assert,tests.tools.test_full_sync,tests.tools.test_run_block,tests.util.alert_server,tests.util.benchmark_cost,tests.util.blockchain,tests.util.build_network_protocol_files,tests.util.db_connection,tests.util.generator_tools_testing,chia.simulator.keyring,tests.util.key_tool,tests.util.test_full_block_utils,tests.util.test_lock_queue,tests.util.test_misc,tests.util.test_network,tests.util.test_network_protocol_files,tests.wallet.cat_wallet.test_cat_lifecycle,tests.wallet.cat_wallet.test_cat_wallet,tests.wallet.cat_wallet.test_offer_lifecycle,tests.wallet.cat_wallet.test_trades,tests.wallet.did_wallet.test_did,tests.wallet.did_wallet.test_did_rpc,tests.wallet.did_wallet.test_nft_rpc,tests.wallet.did_wallet.test_nft_wallet,tests.wallet.rpc.test_wallet_rpc,tests.wallet.simple_sync.test_simple_sync_protocol,tests.wallet.sync.test_wallet_sync,tests.wallet.test_bech32m,tests.wallet.test_chialisp,tests.wallet.test_puzzle_store,tests.wallet.test_singleton,tests.wallet.test_singleton_lifecycle,tests.wallet.test_singleton_lifecycle_fast,tests.wallet.test_taproot,tests.wallet.test_wallet_blockchain,tests.wallet.test_wallet_interested_store,tests.wallet.test_wallet_key_val_store,tests.wallet.test_wallet_user_store,chia.simulator.wallet_tools,tests.weight_proof.test_weight_proof,tools.analyze-chain,tools.run_block,tools.test_full_sync,tests.wallet.nft_wallet.test_nft_wallet,chia.wallet.nft_wallet.nft_puzzles,tests.wallet.nft_wallet.test_nft_puzzles]
 disable_error_code = annotation-unchecked
 disallow_any_generics = False
 disallow_subclassing_any = False
 disallow_untyped_calls = False
 disallow_untyped_defs = False
 disallow_incomplete_defs = False
 check_untyped_defs = False
```

### Comparing `chia-blockchain-1.8.0b6/pylintrc` & `chia-blockchain-1.8.0rc1/pylintrc`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/pytest.ini` & `chia-blockchain-1.8.0rc1/pytest.ini`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/setup.py` & `chia-blockchain-1.8.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "boto3==1.26.111",  # AWS S3 for DL s3 plugin
     "blspy==1.0.16",  # Signature library
     "chiavdf==1.0.8",  # timelord and vdf verification
     "chiabip158==1.2",  # bip158-style wallet filters
     "chiapos==1.0.11",  # proof of space
     "clvm==0.9.7",
     "clvm_tools==0.4.6",  # Currying, Program.to, other conveniences
-    "chia_rs==0.2.5",
+    "chia_rs==0.2.6",
     "clvm-tools-rs==0.1.30",  # Rust implementation of clvm_tools' compiler
     "aiohttp==3.8.4",  # HTTP server for full node rpc
     "aiosqlite==0.17.0",  # asyncio wrapper for sqlite, to store blocks
     "bitstring==4.0.1",  # Binary data management library
     "colorama==0.4.6",  # Colorizes terminal output
     "colorlog==6.7.0",  # Adds color to logs
     "concurrent-log-handler==0.9.20",  # Concurrently log and rotate logs
@@ -142,15 +142,15 @@
             "chia_data_layer = chia.server.start_data_layer:main",
             "chia_data_layer_http = chia.data_layer.data_layer_server:main",
             "chia_data_layer_s3_plugin = chia.data_layer.s3_plugin_service:run_server",
         ]
     },
     package_data={
         "chia": ["pyinstaller.spec"],
-        "": ["*.clvm", "*.clvm.hex", "*.clib", "*.clinc", "*.clsp", "py.typed"],
+        "": ["*.clsp", "*.clsp.hex", "*.clvm", "*.clib", "py.typed"],
         "chia.util": ["initial-*.yaml", "english.txt"],
         "chia.ssl": ["chia_ca.crt", "chia_ca.key", "dst_root_ca.pem"],
         "mozilla-ca": ["cacert.pem"],
     },
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     zip_safe=False,
```

### Comparing `chia-blockchain-1.8.0b6/start-gui.sh` & `chia-blockchain-1.8.0rc1/start-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/README.md` & `chia-blockchain-1.8.0rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/blockchain/blockchain_test_utils.py` & `chia-blockchain-1.8.0rc1/tests/blockchain/blockchain_test_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain.py` & `chia-blockchain-1.8.0rc1/tests/blockchain/test_blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain_transactions.py` & `chia-blockchain-1.8.0rc1/tests/blockchain/test_blockchain_transactions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/build-init-files.py` & `chia-blockchain-1.8.0rc1/tests/build-init-files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/build-job-matrix.py` & `chia-blockchain-1.8.0rc1/tests/build-job-matrix.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/check_pytest_monitor_output.py` & `chia-blockchain-1.8.0rc1/tests/check_pytest_monitor_output.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/check_sql_statements.py` & `chia-blockchain-1.8.0rc1/tests/check_sql_statements.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/chia-start-sim` & `chia-blockchain-1.8.0rc1/tests/chia-start-sim`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/benchmark_costs.py` & `chia-blockchain-1.8.0rc1/tests/clvm/benchmark_costs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/coin_store.py` & `chia-blockchain-1.8.0rc1/tests/clvm/coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_chialisp_deserialization.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_chialisp_deserialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from unittest import TestCase
 
 from chia.types.blockchain_format.program import INFINITE_COST, Program
 from chia.util.byte_types import hexstr_to_bytes
 from chia.wallet.puzzles.load_clvm import load_clvm
 
-DESERIALIZE_MOD = load_clvm("chialisp_deserialisation.clvm", package_or_requirement="chia.wallet.puzzles")
+DESERIALIZE_MOD = load_clvm("chialisp_deserialisation.clsp", package_or_requirement="chia.wallet.puzzles")
 
 
 def serialized_atom_overflow(size):
     if size == 0:
         size_blob = b"\x80"
     elif size < 0x40:
         size_blob = bytes([0x80 | size])
```

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_clvm_step.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_clvm_step.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_curry_and_treehash.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_curry_and_treehash.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_program.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_program.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_compression.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_puzzle_compression.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_drivers.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_puzzle_drivers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_puzzles.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_puzzles.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_serialized_program.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_serialized_program.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from unittest import TestCase
 
 from chia.types.blockchain_format.program import INFINITE_COST, Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.wallet.puzzles.load_clvm import load_clvm
 
-SHA256TREE_MOD = load_clvm("sha256tree_module.clvm")
+SHA256TREE_MOD = load_clvm("sha256tree_module.clsp")
 
 
 # TODO: test multiple args
 class TestSerializedProgram(TestCase):
     def test_tree_hash(self):
         p = SHA256TREE_MOD
         s = SerializedProgram.from_bytes(bytes(SHA256TREE_MOD))
```

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_singletons.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_singletons.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 from chia.wallet.puzzles import p2_conditions, p2_delegated_puzzle_or_hidden_puzzle
 from tests.clvm.test_puzzles import public_key_for_index, secret_exponent_for_index
 from tests.util.key_tool import KeyTool
 
 """
 This test suite aims to test:
     - chia.wallet.puzzles.singleton_top_layer.py
-    - chia.wallet.puzzles.singleton_top_layer.clvm
+    - chia.wallet.puzzles.singleton_top_layer.clsp
     - chia.wallet.puzzles.singleton_top_layer_v1_1.py
-    - chia.wallet.puzzles.singleton_top_layer_v1_1.clvm
-    - chia.wallet.puzzles.p2_singleton.clvm
-    - chia.wallet.puzzles.p2_singleton_or_delayed_puzhash.clvm
+    - chia.wallet.puzzles.singleton_top_layer_v1_1.clsp
+    - chia.wallet.puzzles.p2_singleton.clsp
+    - chia.wallet.puzzles.p2_singleton_or_delayed_puzhash.clsp
 """
 
 
 class TransactionPushError(Exception):
     pass
```

### Comparing `chia-blockchain-1.8.0b6/tests/clvm/test_spend_sim.py` & `chia-blockchain-1.8.0rc1/tests/clvm/test_spend_sim.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/cmds/test_wallet_check.py` & `chia-blockchain-1.8.0rc1/tests/cmds/test_wallet_check.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/conftest.py` & `chia-blockchain-1.8.0rc1/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,25 +120,25 @@
 
     await db_wrapper.close()
     bc1.shut_down()
     db_path.unlink()
 
 
 @pytest.fixture(scope="function")
-def latest_db_version():
+def latest_db_version() -> int:
     return 2
 
 
 @pytest.fixture(scope="function", params=[1, 2])
-def db_version(request):
+def db_version(request) -> int:
     return request.param
 
 
 @pytest.fixture(scope="function", params=[1000000, 3630000, 4000000])
-def softfork_height(request):
+def softfork_height(request) -> int:
     return request.param
 
 
 saved_blocks_version = "rc5"
 
 
 @pytest.fixture(scope="session")
```

### Comparing `chia-blockchain-1.8.0b6/tests/connection_utils.py` & `chia-blockchain-1.8.0rc1/tests/connection_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/cmds/test_beta.py` & `chia-blockchain-1.8.0rc1/tests/core/cmds/test_beta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/cmds/test_keys.py` & `chia-blockchain-1.8.0rc1/tests/core/cmds/test_keys.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/cmds/test_wallet.py` & `chia-blockchain-1.8.0rc1/tests/core/cmds/test_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/consensus/test_pot_iterations.py` & `chia-blockchain-1.8.0rc1/tests/core/consensus/test_pot_iterations.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/custom_types/test_coin.py` & `chia-blockchain-1.8.0rc1/tests/core/custom_types/test_coin.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/custom_types/test_proof_of_space.py` & `chia-blockchain-1.8.0rc1/tests/core/custom_types/test_proof_of_space.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/custom_types/test_spend_bundle.py` & `chia-blockchain-1.8.0rc1/tests/core/custom_types/test_spend_bundle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon.py` & `chia-blockchain-1.8.0rc1/tests/core/daemon/test_daemon.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon_register.py` & `chia-blockchain-1.8.0rc1/tests/core/daemon/test_daemon_register.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/daemon/test_keychain_proxy.py` & `chia-blockchain-1.8.0rc1/tests/core/daemon/test_keychain_proxy.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/data_layer/conftest.py` & `chia-blockchain-1.8.0rc1/tests/core/data_layer/conftest.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_cli.py` & `chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_cli.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_layer_util.py` & `chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_layer_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_rpc.py` & `chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store.py` & `chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store_schema.py` & `chia-blockchain-1.8.0rc1/tests/core/data_layer/test_data_store_schema.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/data_layer/util.py` & `chia-blockchain-1.8.0rc1/tests/core/data_layer/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/conftest.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/conftest.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/test_full_sync.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/full_sync/test_full_sync.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/ram_db.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/ram_db.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_block_store.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_block_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_coin_store.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_full_node_store.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_full_node_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_hint_store.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_hint_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_sync_store.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/stores/test_sync_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_address_manager.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_address_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_block_height_map.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_block_height_map.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_conditions.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_conditions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_full_node.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_full_node.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_generator_tools.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_generator_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_hint_management.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_hint_management.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_node_load.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_node_load.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_peer_store_resolver.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_peer_store_resolver.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_performance.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_performance.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_subscriptions.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_transactions.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_transactions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/full_node/test_tx_processing_queue.py` & `chia-blockchain-1.8.0rc1/tests/core/full_node/test_tx_processing_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/large_block.py` & `chia-blockchain-1.8.0rc1/tests/core/large_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/make_block_generator.py` & `chia-blockchain-1.8.0rc1/tests/core/make_block_generator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool.py` & `chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_estimator.py` & `chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_fee_estimator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_protocol.py` & `chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_fee_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_manager.py` & `chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_performance.py` & `chia-blockchain-1.8.0rc1/tests/core/mempool/test_mempool_performance.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/node_height.py` & `chia-blockchain-1.8.0rc1/tests/core/node_height.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/flood.py` & `chia-blockchain-1.8.0rc1/tests/core/server/flood.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/serve.py` & `chia-blockchain-1.8.0rc1/tests/core/server/serve.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/test_capabilities.py` & `chia-blockchain-1.8.0rc1/tests/core/server/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/test_dos.py` & `chia-blockchain-1.8.0rc1/tests/core/server/test_dos.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/test_event_loop.py` & `chia-blockchain-1.8.0rc1/tests/core/server/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/test_loop.py` & `chia-blockchain-1.8.0rc1/tests/core/server/test_loop.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/test_rate_limits.py` & `chia-blockchain-1.8.0rc1/tests/core/server/test_rate_limits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/server/test_server.py` & `chia-blockchain-1.8.0rc1/tests/core/server/test_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/ssl/test_ssl.py` & `chia-blockchain-1.8.0rc1/tests/core/ssl/test_ssl.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_coins.py` & `chia-blockchain-1.8.0rc1/tests/core/test_coins.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_cost_calculation.py` & `chia-blockchain-1.8.0rc1/tests/core/test_cost_calculation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_crawler_rpc.py` & `chia-blockchain-1.8.0rc1/tests/core/test_crawler_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_daemon_rpc.py` & `chia-blockchain-1.8.0rc1/tests/core/test_daemon_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_db_conversion.py` & `chia-blockchain-1.8.0rc1/tests/core/test_db_conversion.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_db_validation.py` & `chia-blockchain-1.8.0rc1/tests/core/test_db_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_farmer_harvester_rpc.py` & `chia-blockchain-1.8.0rc1/tests/core/test_farmer_harvester_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_filter.py` & `chia-blockchain-1.8.0rc1/tests/core/test_filter.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_full_node_rpc.py` & `chia-blockchain-1.8.0rc1/tests/core/test_full_node_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_merkle_set.py` & `chia-blockchain-1.8.0rc1/tests/core/test_merkle_set.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/test_services.py` & `chia-blockchain-1.8.0rc1/tests/core/test_services.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_cached_bls.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_cached_bls.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_config.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_file_keyring_synchronization.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_file_keyring_synchronization.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_files.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_jsonify.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_jsonify.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_keychain.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_keychain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_keyring_wrapper.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_keyring_wrapper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_lockfile.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_lru_cache.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_significant_bits.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_significant_bits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/core/util/test_streamable.py` & `chia-blockchain-1.8.0rc1/tests/core/util/test_streamable.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/db/test_db_wrapper.py` & `chia-blockchain-1.8.0rc1/tests/db/test_db_wrapper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/farmer_harvester/test_farmer_harvester.py` & `chia-blockchain-1.8.0rc1/tests/farmer_harvester/test_farmer_harvester.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/fee_estimation/cmdline_test.py` & `chia-blockchain-1.8.0rc1/tests/fee_estimation/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_integration.py` & `chia-blockchain-1.8.0rc1/tests/fee_estimation/test_fee_estimation_integration.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_rpc.py` & `chia-blockchain-1.8.0rc1/tests/fee_estimation/test_fee_estimation_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_unit_tests.py` & `chia-blockchain-1.8.0rc1/tests/fee_estimation/test_fee_estimation_unit_tests.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/fee_estimation/test_mempoolitem_height_added.py` & `chia-blockchain-1.8.0rc1/tests/fee_estimation/test_mempoolitem_height_added.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/generator/test_compression.py` & `chia-blockchain-1.8.0rc1/tests/generator/test_compression.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # flake8: noqa: F501
 from __future__ import annotations
 
 import io
 from dataclasses import dataclass
 from typing import Any, List
-from unittest import TestCase
 
+import pytest
 from clvm import SExp
 from clvm.serialize import sexp_from_stream
 from clvm_tools import binutils
 
 from chia.full_node.bundle_tools import (
     bundle_suitable_for_compression,
     compressed_coin_spend_entry_list,
     compressed_spend_bundle_solution,
     match_standard_transaction_at_any_index,
     simple_solution_generator,
     spend_bundle_to_serialized_coin_spend_entry_list,
 )
-from chia.full_node.generator import create_generator_args, run_generator_unsafe
 from chia.full_node.mempool_check_conditions import get_puzzle_and_solution_for_coin
 from chia.types.blockchain_format.program import INFINITE_COST, Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.generator_types import BlockGenerator, CompressorArg
 from chia.types.spend_bundle import SpendBundle
 from chia.util.byte_types import hexstr_to_bytes
 from chia.util.ints import uint32
 from chia.wallet.puzzles.load_clvm import load_clvm
 from tests.core.make_block_generator import make_spend_bundle
+from tests.generator.test_rom import run_generator
 
-TEST_GEN_DESERIALIZE = load_clvm("test_generator_deserialize.clvm", package_or_requirement="chia.wallet.puzzles")
-DESERIALIZE_MOD = load_clvm("chialisp_deserialisation.clvm", package_or_requirement="chia.wallet.puzzles")
+TEST_GEN_DESERIALIZE = load_clvm("test_generator_deserialize.clsp", package_or_requirement="chia.wallet.puzzles")
+DESERIALIZE_MOD = load_clvm("chialisp_deserialisation.clsp", package_or_requirement="chia.wallet.puzzles")
 
-DECOMPRESS_PUZZLE = load_clvm("decompress_puzzle.clvm", package_or_requirement="chia.wallet.puzzles")
-DECOMPRESS_CSE = load_clvm("decompress_coin_spend_entry.clvm", package_or_requirement="chia.wallet.puzzles")
+DECOMPRESS_PUZZLE = load_clvm("decompress_puzzle.clsp", package_or_requirement="chia.wallet.puzzles")
+DECOMPRESS_CSE = load_clvm("decompress_coin_spend_entry.clsp", package_or_requirement="chia.wallet.puzzles")
 
 DECOMPRESS_CSE_WITH_PREFIX = load_clvm(
-    "decompress_coin_spend_entry_with_prefix.clvm", package_or_requirement="chia.wallet.puzzles"
+    "decompress_coin_spend_entry_with_prefix.clsp", package_or_requirement="chia.wallet.puzzles"
 )
-DECOMPRESS_BLOCK = load_clvm("block_program_zero.clvm", package_or_requirement="chia.wallet.puzzles")
-TEST_MULTIPLE = load_clvm("test_multiple_generator_input_arguments.clvm", package_or_requirement="chia.wallet.puzzles")
+DECOMPRESS_BLOCK = load_clvm("block_program_zero.clsp", package_or_requirement="chia.wallet.puzzles")
+TEST_MULTIPLE = load_clvm("test_multiple_generator_input_arguments.clsp", package_or_requirement="chia.wallet.puzzles")
 
 Nil = Program.from_bytes(b"\x80")
 
 original_generator = hexstr_to_bytes(
     "ff01ffffffa00000000000000000000000000000000000000000000000000000000000000000ff830186a080ffffff02ffff01ff02ffff01ff02ffff03ff0bffff01ff02ffff03ffff09ff05ffff1dff0bffff1effff0bff0bffff02ff06ffff04ff02ffff04ff17ff8080808080808080ffff01ff02ff17ff2f80ffff01ff088080ff0180ffff01ff04ffff04ff04ffff04ff05ffff04ffff02ff06ffff04ff02ffff04ff17ff80808080ff80808080ffff02ff17ff2f808080ff0180ffff04ffff01ff32ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff06ffff04ff02ffff04ff09ff80808080ffff02ff06ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff018080ffff04ffff01b081963921826355dcb6c355ccf9c2637c18adf7d38ee44d803ea9ca41587e48c913d8d46896eb830aeadfc13144a8eac3ff018080ffff80ffff01ffff33ffa06b7a83babea1eec790c947db4464ab657dbe9b887fe9acc247062847b8c2a8a9ff830186a08080ff8080808080"
 )  # noqa
 
@@ -95,166 +95,179 @@
             coin_spend.coin.amount,
             sexp_from_stream(io.BytesIO(bytes(coin_spend.solution)), SExp.to),
         ]
         r.append(entry)
     return r
 
 
-class TestCompression(TestCase):
-    def test_spend_bundle_suitable(self):
+class TestCompression:
+    def test_spend_bundle_suitable(self) -> None:
         sb: SpendBundle = make_spend_bundle(1)
         assert bundle_suitable_for_compression(sb)
 
-    def test_compress_spend_bundle(self):
+    def test_compress_spend_bundle(self) -> None:
         pass
 
-    def test_multiple_input_gen_refs(self):
-        start1, end1 = match_standard_transaction_at_any_index(gen1)
-        start2, end2 = match_standard_transaction_at_any_index(gen2)
+    def test_multiple_input_gen_refs(self) -> None:
+        match = match_standard_transaction_at_any_index(gen1)
+        assert match is not None
+        start1, end1 = match
+        match = match_standard_transaction_at_any_index(gen2)
+        assert match is not None
+        start2, end2 = match
         ca1 = CompressorArg(FAKE_BLOCK_HEIGHT1, SerializedProgram.from_bytes(gen1), start1, end1)
         ca2 = CompressorArg(FAKE_BLOCK_HEIGHT2, SerializedProgram.from_bytes(gen2), start2, end2)
 
         prefix_len1 = end1 - start1
         prefix_len2 = end2 - start2
         assert prefix_len1 == prefix_len2
         prefix_len = prefix_len1
         results = []
         for split_offset in range(prefix_len):
             gen_args = MultipleCompressorArg([ca1, ca2], split_offset)
             spend_bundle: SpendBundle = make_spend_bundle(1)
             multi_gen = create_multiple_ref_generator(gen_args, spend_bundle)
-            cost, result = run_generator_unsafe(multi_gen, INFINITE_COST)
+            cost, result = run_generator(multi_gen)
             results.append(result)
             assert result is not None
             assert cost > 0
         assert all(r == results[0] for r in results)
 
-    def test_compressed_block_results(self):
+    def test_compressed_block_results(self) -> None:
         sb: SpendBundle = make_spend_bundle(1)
-        start, end = match_standard_transaction_at_any_index(original_generator)
+        match = match_standard_transaction_at_any_index(original_generator)
+        assert match is not None
+        start, end = match
         ca = CompressorArg(uint32(0), SerializedProgram.from_bytes(original_generator), start, end)
         c = compressed_spend_bundle_solution(ca, sb)
         s = simple_solution_generator(sb)
         assert c != s
-        cost_c, result_c = run_generator_unsafe(c, INFINITE_COST)
-        cost_s, result_s = run_generator_unsafe(s, INFINITE_COST)
+        cost_c, result_c = run_generator(c)
+        cost_s, result_s = run_generator(s)
+        print()
         print(result_c)
         assert result_c is not None
         assert result_s is not None
+        print(result_s)
         assert result_c == result_s
 
-    def test_get_removals_for_single_coin(self):
+    def test_get_removals_for_single_coin(self) -> None:
         sb: SpendBundle = make_spend_bundle(1)
-        start, end = match_standard_transaction_at_any_index(original_generator)
+        match = match_standard_transaction_at_any_index(original_generator)
+        assert match is not None
+        start, end = match
         ca = CompressorArg(uint32(0), SerializedProgram.from_bytes(original_generator), start, end)
         c = compressed_spend_bundle_solution(ca, sb)
         removal = sb.coin_spends[0].coin
         error, puzzle, solution = get_puzzle_and_solution_for_coin(c, removal)
         assert error is None
+        assert puzzle is not None
+        assert solution is not None
         assert bytes(puzzle) == bytes(sb.coin_spends[0].puzzle_reveal)
         assert bytes(solution) == bytes(sb.coin_spends[0].solution)
         # Test non compressed generator as well
         s = simple_solution_generator(sb)
         error, puzzle, solution = get_puzzle_and_solution_for_coin(s, removal)
         assert error is None
+        assert puzzle is not None
+        assert solution is not None
         assert bytes(puzzle) == bytes(sb.coin_spends[0].puzzle_reveal)
         assert bytes(solution) == bytes(sb.coin_spends[0].solution)
 
-    def test_spend_byndle_coin_spend(self):
+    def test_spend_byndle_coin_spend(self) -> None:
         for i in range(0, 10):
             sb: SpendBundle = make_spend_bundle(i)
             cs1 = SExp.to(spend_bundle_to_coin_spend_entry_list(sb)).as_bin()  # pylint: disable=E1101
             cs2 = spend_bundle_to_serialized_coin_spend_entry_list(sb)
             assert cs1 == cs2
 
 
-class TestDecompression(TestCase):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+class TestDecompression:
+    def __init__(self) -> None:
         self.maxDiff = None
 
-    def test_deserialization(self):
+    def test_deserialization(self) -> None:
         self.maxDiff = None
         cost, out = DESERIALIZE_MOD.run_with_cost(INFINITE_COST, [bytes(Program.to("hello"))])
         assert out == Program.to("hello")
 
-    def test_deserialization_as_argument(self):
+    def test_deserialization_as_argument(self) -> None:
         self.maxDiff = None
         cost, out = TEST_GEN_DESERIALIZE.run_with_cost(
             INFINITE_COST, [DESERIALIZE_MOD, Nil, bytes(Program.to("hello"))]
         )
         print(bytes(Program.to("hello")))
         print()
         print(out)
         assert out == Program.to("hello")
 
-    def test_decompress_puzzle(self):
+    def test_decompress_puzzle(self) -> None:
         cost, out = DECOMPRESS_PUZZLE.run_with_cost(
             INFINITE_COST, [DESERIALIZE_MOD, b"\xff", bytes(Program.to("pubkey")), b"\x80"]
         )
 
         print()
         print(out)
 
     # An empty CSE is invalid. (An empty CSE list may be okay)
     # def test_decompress_empty_cse(self):
     #    cse0 = binutils.assemble("()")
     #    cost, out = DECOMPRESS_CSE.run_with_cost(INFINITE_COST, [DESERIALIZE_MOD, DECOMPRESS_PUZZLE, b"\xff", b"\x80", cse0])
     #    print()
     #    print(out)
 
-    def test_decompress_cse(self):
+    def test_decompress_cse(self) -> None:
         """Decompress a single CSE / CoinSpendEntry"""
         cse0 = binutils.assemble(
             "((0x0000000000000000000000000000000000000000000000000000000000000000 0x0186a0) (0xb081963921826355dcb6c355ccf9c2637c18adf7d38ee44d803ea9ca41587e48c913d8d46896eb830aeadfc13144a8eac3 (() (q (51 0x6b7a83babea1eec790c947db4464ab657dbe9b887fe9acc247062847b8c2a8a9 0x0186a0)) ())))"
-        )  # noqa
+        )  # type: ignore[no-untyped-call]
         cost, out = DECOMPRESS_CSE.run_with_cost(
             INFINITE_COST, [DESERIALIZE_MOD, DECOMPRESS_PUZZLE, b"\xff", b"\x80", cse0]
         )
 
         print()
         print(out)
 
-    def test_decompress_cse_with_prefix(self):
+    def test_decompress_cse_with_prefix(self) -> None:
         cse0 = binutils.assemble(
             "((0x0000000000000000000000000000000000000000000000000000000000000000 0x0186a0) (0xb081963921826355dcb6c355ccf9c2637c18adf7d38ee44d803ea9ca41587e48c913d8d46896eb830aeadfc13144a8eac3 (() (q (51 0x6b7a83babea1eec790c947db4464ab657dbe9b887fe9acc247062847b8c2a8a9 0x0186a0)) ())))"
-        )  # noqa
+        )  # type: ignore[no-untyped-call]
 
         start = 2 + 44
         end = start + 238
         prefix = original_generator[start:end]
         # (deserialize decompress_puzzle puzzle_prefix cse)
         cost, out = DECOMPRESS_CSE_WITH_PREFIX.run_with_cost(
             INFINITE_COST, [DESERIALIZE_MOD, DECOMPRESS_PUZZLE, prefix, cse0]
         )
 
         print()
         print(out)
 
-    def test_block_program_zero(self):
+    def test_block_program_zero(self) -> None:
         "Decompress a list of CSEs"
         self.maxDiff = None
         cse1 = binutils.assemble(
             "(((0x0000000000000000000000000000000000000000000000000000000000000000 0x0186a0) (0xb081963921826355dcb6c355ccf9c2637c18adf7d38ee44d803ea9ca41587e48c913d8d46896eb830aeadfc13144a8eac3 (() (q (51 0x6b7a83babea1eec790c947db4464ab657dbe9b887fe9acc247062847b8c2a8a9 0x0186a0)) ()))))"
-        )  # noqa
+        )  # type: ignore[no-untyped-call]
         cse2 = binutils.assemble(
             """
 (
   ((0x0000000000000000000000000000000000000000000000000000000000000000 0x0186a0)
    (0xb081963921826355dcb6c355ccf9c2637c18adf7d38ee44d803ea9ca41587e48c913d8d46896eb830aeadfc13144a8eac3
     (() (q (51 0x6b7a83babea1eec790c947db4464ab657dbe9b887fe9acc247062847b8c2a8a9 0x0186a0)) ()))
   )
 
   ((0x0000000000000000000000000000000000000000000000000000000000000001 0x0186a0)
    (0xb0a6207f5173ec41491d9f2c1b8fff5579e13703077e0eaca8fe587669dcccf51e9209a6b65576845ece5f7c2f3229e7e3
    (() (q (51 0x24254a3efc3ebfac9979bbe0d615e2eda043aa329905f65b63846fa24149e2b6 0x0186a0)) ())))
 
 )
         """
-        )  # noqa
+        )  # type: ignore[no-untyped-call]
 
         start = 2 + 44
         end = start + 238
 
         # (mod (decompress_puzzle decompress_coin_spend_entry start end compressed_cses deserialize generator_list reserved_arg)
         # cost, out = DECOMPRESS_BLOCK.run_with_cost(INFINITE_COST, [DECOMPRESS_PUZZLE, DECOMPRESS_CSE, start, Program.to(end), cse0, DESERIALIZE_MOD, bytes(original_generator)])
         cost, out = DECOMPRESS_BLOCK.run_with_cost(
@@ -269,34 +282,34 @@
                 [bytes(original_generator)],
             ],
         )
 
         print()
         print(out)
 
-    def test_block_program_zero_with_curry(self):
+    def test_block_program_zero_with_curry(self) -> None:
         self.maxDiff = None
         cse1 = binutils.assemble(
             "(((0x0000000000000000000000000000000000000000000000000000000000000000 0x0186a0) (0xb081963921826355dcb6c355ccf9c2637c18adf7d38ee44d803ea9ca41587e48c913d8d46896eb830aeadfc13144a8eac3 (() (q (51 0x6b7a83babea1eec790c947db4464ab657dbe9b887fe9acc247062847b8c2a8a9 0x0186a0)) ()))))"
-        )  # noqa
+        )  # type: ignore[no-untyped-call]
         cse2 = binutils.assemble(
             """
 (
   ((0x0000000000000000000000000000000000000000000000000000000000000000 0x0186a0)
    (0xb081963921826355dcb6c355ccf9c2637c18adf7d38ee44d803ea9ca41587e48c913d8d46896eb830aeadfc13144a8eac3
     (() (q (51 0x6b7a83babea1eec790c947db4464ab657dbe9b887fe9acc247062847b8c2a8a9 0x0186a0)) ()))
   )
 
   ((0x0000000000000000000000000000000000000000000000000000000000000001 0x0186a0)
    (0xb0a6207f5173ec41491d9f2c1b8fff5579e13703077e0eaca8fe587669dcccf51e9209a6b65576845ece5f7c2f3229e7e3
    (() (q (51 0x24254a3efc3ebfac9979bbe0d615e2eda043aa329905f65b63846fa24149e2b6 0x0186a0)) ())))
 
 )
         """
-        )  # noqa
+        )  # type: ignore[no-untyped-call]
 
         start = 2 + 44
         end = start + 238
 
         # (mod (decompress_puzzle decompress_coin_spend_entry start end compressed_cses deserialize generator_list reserved_arg)
         # cost, out = DECOMPRESS_BLOCK.run_with_cost(INFINITE_COST, [DECOMPRESS_PUZZLE, DECOMPRESS_CSE, start, Program.to(end), cse0, DESERIALIZE_MOD, bytes(original_generator)])
         p = DECOMPRESS_BLOCK.curry(DECOMPRESS_PUZZLE, DECOMPRESS_CSE_WITH_PREFIX, start, Program.to(end))
@@ -305,13 +318,13 @@
         print()
         print(p)
         print(out)
 
         p_with_cses = DECOMPRESS_BLOCK.curry(
             DECOMPRESS_PUZZLE, DECOMPRESS_CSE_WITH_PREFIX, start, Program.to(end), cse2, DESERIALIZE_MOD
         )
-        generator_args = create_generator_args([SerializedProgram.from_bytes(original_generator)])
+        generator_args = Program.to([[original_generator]])
         cost, out = p_with_cses.run_with_cost(INFINITE_COST, generator_args)
 
         print()
         print(p_with_cses)
         print(out)
```

### Comparing `chia-blockchain-1.8.0b6/tests/generator/test_generator_types.py` & `chia-blockchain-1.8.0rc1/tests/generator/test_generator_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Dict
 from unittest import TestCase
 
-from chia.full_node.generator import create_block_generator, create_generator_args
+from chia.full_node.generator import create_block_generator
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.generator_types import GeneratorBlockCacheInterface
 from chia.util.ints import uint32
 
 gen0 = SerializedProgram.from_bytes(
     bytes.fromhex(
@@ -33,26 +33,24 @@
         self.d = d
 
     def get_generator_for_block_height(self, index: uint32) -> SerializedProgram:
         return self.d[index]
 
 
 class TestGeneratorTypes(TestCase):
-    def test_make_generator(self):
+    def test_make_generator(self) -> None:
         block_dict = BlockDict({uint32(1): gen1})
         gen = create_block_generator(gen2, [uint32(1)], block_dict)
         print(gen)
 
-    def test_make_generator_args(self):
-        generator_ref_list = [gen1]
-        gen_args = create_generator_args(generator_ref_list)
-        gen_args_as_program = Program.from_bytes(bytes(gen_args))
+    def test_make_generator_args(self) -> None:
+        gen_args = Program.to([[bytes(gen1)]])
 
         # First Argument to the block generator is the first template generator
-        arg2 = gen_args_as_program.first().first()
+        arg2 = gen_args.first().first()
         print(arg2)
         assert arg2 == bytes(gen1)
 
     # It's not a list anymore.
     # TODO: Test the first three arg positions passed through here.
     # def test_generator_arg_is_list(self):
     #    generator_ref_list = [Program.to(b"gen1"), Program.to(b"gen2")]
```

### Comparing `chia-blockchain-1.8.0b6/tests/generator/test_list_to_batches.py` & `chia-blockchain-1.8.0rc1/tests/generator/test_list_to_batches.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/generator/test_rom.py` & `chia-blockchain-1.8.0rc1/tests/generator/test_rom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
-from typing import List
+from typing import List, Tuple
 
 from clvm_tools import binutils
 from clvm_tools.clvmc import compile_clvm_text
 
 from chia.consensus.condition_costs import ConditionCost
-from chia.full_node.generator import run_generator_unsafe
 from chia.full_node.mempool_check_conditions import get_name_puzzle_conditions
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.generator_types import BlockGenerator
 from chia.types.spend_bundle_conditions import ELIGIBLE_FOR_DEDUP, Spend
 from chia.util.ints import uint32
 from chia.wallet.puzzles.load_clvm import load_clvm
+from chia.wallet.puzzles.rom_bootstrap_generator import GENERATOR_MOD
 
 MAX_COST = int(1e15)
 COST_PER_BYTE = int(12000)
 
 
-DESERIALIZE_MOD = load_clvm("chialisp_deserialisation.clvm", package_or_requirement="chia.wallet.puzzles")
+DESERIALIZE_MOD = load_clvm("chialisp_deserialisation.clsp", package_or_requirement="chia.wallet.puzzles")
 
 
 GENERATOR_CODE = """
 (mod (deserialize-mod historical-generators)
     (defun first-block (deserialize-mod historical-generators)
                        (a deserialize-mod (list (f historical-generators))))
 
@@ -42,36 +42,39 @@
 
 COMPILED_GENERATOR_CODE = bytes.fromhex(
     "ff02ffff01ff04ffff02ff04ffff04ff02ffff04ff05ffff04ff0bff8080808080ffff02"
     "ff06ffff04ff02ffff04ff05ffff04ff0bff808080808080ffff04ffff01ffff02ff05ff"
     "1380ff02ff05ff2b80ff018080"
 )
 
-COMPILED_GENERATOR_CODE = bytes(Program.to(compile_clvm_text(GENERATOR_CODE, [])))
+COMPILED_GENERATOR_CODE = bytes(Program.to(compile_clvm_text(GENERATOR_CODE, [])))  # type: ignore[no-untyped-call]
 
 FIRST_GENERATOR = Program.to(
-    binutils.assemble('((parent_id (c 1 (q "puzzle blob")) 50000 "solution is here" extra data for coin))')
+    binutils.assemble(
+        '((parent_id (c 1 (q "puzzle blob")) 50000 "solution is here" extra data for coin))'
+    )  # type: ignore[no-untyped-call]
 ).as_bin()
 
-SECOND_GENERATOR = Program.to(binutils.assemble("(extra data for block)")).as_bin()
+SECOND_GENERATOR = Program.to(binutils.assemble("(extra data for block)")).as_bin()  # type: ignore[no-untyped-call]
 
 
 FIRST_GENERATOR = Program.to(
     binutils.assemble(
         """
         ((0x0000000000000000000000000000000000000000000000000000000000000000 1 50000
-        ((51 0x0000000000000000000000000000000000000000000000000000000000000001 500)) "extra" "data" "for" "coin" ))"""
+        ((51 0x0000000000000000000000000000000000000000000000000000000000000001 500))
+        "extra" "data" "for" "coin" ))"""  # type: ignore[no-untyped-call]
     )
 ).as_bin()
 
-SECOND_GENERATOR = Program.to(binutils.assemble("(extra data for block)")).as_bin()
+SECOND_GENERATOR = Program.to(binutils.assemble("(extra data for block)")).as_bin()  # type: ignore[no-untyped-call]
 
 
-def to_sp(sexp) -> SerializedProgram:
-    return SerializedProgram.from_bytes(bytes(sexp))
+def to_sp(sexp: bytes) -> SerializedProgram:
+    return SerializedProgram.from_bytes(sexp)
 
 
 def block_generator() -> BlockGenerator:
     generator_list = [to_sp(FIRST_GENERATOR), to_sp(SECOND_GENERATOR)]
     generator_heights = [uint32(0), uint32(1)]
     return BlockGenerator(to_sp(COMPILED_GENERATOR_CODE), generator_list, generator_heights)
 
@@ -82,14 +85,20 @@
     "ffffffa00000000000000000000000000000000000000000000000000000000000000000"
     "ff01ff8300c350ffffff33ffa00000000000000000000000000000000000000000000000"
     "000000000000000001ff8201f48080ff856578747261ff8464617461ff83666f72ff8463"
     "6f696e8080ff856578747261ff8464617461ff83666f72ff85626c6f636b80"
 )
 
 
+def run_generator(self: BlockGenerator) -> Tuple[int, Program]:
+    """This mode is meant for accepting possibly soft-forked transactions into the mempool"""
+    args = Program.to([[bytes(g) for g in self.generator_refs]])
+    return GENERATOR_MOD.run_with_cost(MAX_COST, self.program, args)
+
+
 def as_atom_list(prg: Program) -> List[bytes]:
     """
     Pretend `prg` is a list of atoms. Return the corresponding
     python list of atoms.
 
     At each step, we always assume a node to be an atom or a pair.
     If the assumption is wrong, we exit early. This way we never fail
@@ -106,36 +115,39 @@
             break
         items.append(atom)
         obj = pair[1]
     return items
 
 
 class TestROM:
-    def test_rom_inputs(self):
+    def test_rom_inputs(self) -> None:
         # this test checks that the generator just works
         # It's useful for debugging the generator prior to having the ROM invoke it.
 
         args = Program.to([DESERIALIZE_MOD, [FIRST_GENERATOR, SECOND_GENERATOR]])
         sp = to_sp(COMPILED_GENERATOR_CODE)
         cost, r = sp.run_with_cost(MAX_COST, args)
         assert cost == EXPECTED_ABBREVIATED_COST
         assert r.as_bin().hex() == EXPECTED_OUTPUT
 
-    def test_get_name_puzzle_conditions(self, softfork_height):
+    def test_get_name_puzzle_conditions(self, softfork_height: int) -> None:
         # this tests that extra block or coin data doesn't confuse `get_name_puzzle_conditions`
 
         gen = block_generator()
-        cost, r = run_generator_unsafe(gen, max_cost=MAX_COST)
+        cost, r = run_generator(gen)
         print(r)
 
-        npc_result = get_name_puzzle_conditions(gen, max_cost=MAX_COST, mempool_mode=False, height=softfork_height)
+        npc_result = get_name_puzzle_conditions(
+            gen, max_cost=MAX_COST, mempool_mode=False, height=uint32(softfork_height)
+        )
         assert npc_result.error is None
         assert npc_result.cost == EXPECTED_COST + ConditionCost.CREATE_COIN.value + (
             len(bytes(gen.program)) * COST_PER_BYTE
         )
+        assert npc_result.conds is not None
 
         spend = Spend(
             coin_id=bytes32.fromhex("e8538c2d14f2a7defae65c5c97f5d4fae7ee64acef7fec9d28ad847a0880fd03"),
             puzzle_hash=bytes32.fromhex("9dcf97a184f32623d11a73124ceb99a5709b083721e878a16d78f596718ba7b2"),
             height_relative=None,
             seconds_relative=None,
             before_height_relative=None,
@@ -145,24 +157,24 @@
             create_coin=[(bytes([0] * 31 + [1]), 500, None)],
             agg_sig_me=[],
             flags=ELIGIBLE_FOR_DEDUP,
         )
 
         assert npc_result.conds.spends == [spend]
 
-    def test_coin_extras(self):
+    def test_coin_extras(self) -> None:
         # the ROM supports extra data after a coin. This test checks that it actually gets passed through
 
         gen = block_generator()
-        cost, r = run_generator_unsafe(gen, max_cost=MAX_COST)
+        cost, r = run_generator(gen)
         coin_spends = r.first()
         for coin_spend in coin_spends.as_iter():
             extra_data = coin_spend.rest().rest().rest().rest()
             assert as_atom_list(extra_data) == b"extra data for coin".split()
 
-    def test_block_extras(self):
+    def test_block_extras(self) -> None:
         # the ROM supports extra data after the coin spend list. This test checks that it actually gets passed through
 
         gen = block_generator()
-        cost, r = run_generator_unsafe(gen, max_cost=MAX_COST)
+        cost, r = run_generator(gen)
         extra_block_data = r.rest()
         assert as_atom_list(extra_block_data) == b"extra data for block".split()
```

### Comparing `chia-blockchain-1.8.0b6/tests/generator/test_scan.py` & `chia-blockchain-1.8.0rc1/tests/generator/test_scan.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/plot_sync/test_delta.py` & `chia-blockchain-1.8.0rc1/tests/plot_sync/test_delta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/plot_sync/test_plot_sync.py` & `chia-blockchain-1.8.0rc1/tests/plot_sync/test_plot_sync.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/plot_sync/test_receiver.py` & `chia-blockchain-1.8.0rc1/tests/plot_sync/test_receiver.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/plot_sync/test_sender.py` & `chia-blockchain-1.8.0rc1/tests/plot_sync/test_sender.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/plot_sync/test_sync_simulated.py` & `chia-blockchain-1.8.0rc1/tests/plot_sync/test_sync_simulated.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/plot_sync/util.py` & `chia-blockchain-1.8.0rc1/tests/plot_sync/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/plotting/test_plot_manager.py` & `chia-blockchain-1.8.0rc1/tests/plotting/test_plot_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/pools/test_pool_cmdline.py` & `chia-blockchain-1.8.0rc1/tests/pools/test_pool_cmdline.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/pools/test_pool_config.py` & `chia-blockchain-1.8.0rc1/tests/pools/test_pool_config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/pools/test_pool_puzzles_lifecycle.py` & `chia-blockchain-1.8.0rc1/tests/pools/test_pool_puzzles_lifecycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 from tests.clvm.coin_store import BadSpendBundleError, CoinStore, CoinTimestamp
 from tests.clvm.test_puzzles import public_key_for_index, secret_exponent_for_index
 from tests.util.key_tool import KeyTool
 
 """
 This test suite aims to test:
     - chia.pools.pool_puzzles.py
-    - chia.wallet.puzzles.pool_member_innerpuz.clvm
-    - chia.wallet.puzzles.pool_waiting_room_innerpuz.clvm
+    - chia.wallet.puzzles.pool_member_innerpuz.clsp
+    - chia.wallet.puzzles.pool_waiting_room_innerpuz.clsp
 """
 
 
 # Helper function
 def sign_delegated_puz(del_puz: Program, coin: Coin) -> G2Element:
     synthetic_secret_key: PrivateKey = calculate_synthetic_secret_key(
         PrivateKey.from_bytes(
```

### Comparing `chia-blockchain-1.8.0b6/tests/pools/test_pool_rpc.py` & `chia-blockchain-1.8.0rc1/tests/pools/test_pool_rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,24 +59,23 @@
 async def manage_temporary_pool_plot(
     bt: BlockTools,
     p2_singleton_puzzle_hash: bytes32,
 ) -> AsyncIterator[TemporaryPoolPlot]:
     with tempfile.TemporaryDirectory() as tmpdir:
         tmp_path: Path = Path(tmpdir)
         bt.add_plot_directory(tmp_path)
-        plot_id = await bt.new_plot(p2_singleton_puzzle_hash, tmp_path, tmp_dir=tmp_path)
-        assert plot_id is not None
+        bt_plot = await bt.new_plot(p2_singleton_puzzle_hash, tmp_path, tmp_dir=tmp_path)
         await bt.refresh_plots()
 
-        plot = TemporaryPoolPlot(bt=bt, p2_singleton_puzzle_hash=p2_singleton_puzzle_hash, plot_id=plot_id)
+        plot = TemporaryPoolPlot(bt=bt, p2_singleton_puzzle_hash=p2_singleton_puzzle_hash, plot_id=bt_plot.plot_id)
 
         try:
             yield plot
         finally:
-            await bt.delete_plot(plot_id)
+            await bt.delete_plot(bt_plot.plot_id)
 
 
 PREFARMED_BLOCKS = 4
 
 
 @pytest.fixture(scope="function", params=[False, True])
 def trusted(request: SubRequest) -> bool:
```

### Comparing `chia-blockchain-1.8.0b6/tests/pools/test_pool_wallet.py` & `chia-blockchain-1.8.0rc1/tests/pools/test_pool_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/pools/test_wallet_pool_store.py` & `chia-blockchain-1.8.0rc1/tests/pools/test_wallet_pool_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/simulation/test_simulation.py` & `chia-blockchain-1.8.0rc1/tests/simulation/test_simulation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/simulation/test_simulator.py` & `chia-blockchain-1.8.0rc1/tests/simulation/test_simulator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/simulation/test_start_simulator.py` & `chia-blockchain-1.8.0rc1/tests/simulation/test_start_simulator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/1315537.json` & `chia-blockchain-1.8.0rc1/tests/tools/1315537.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/1315544.json` & `chia-blockchain-1.8.0rc1/tests/tools/1315544.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/1315630.json` & `chia-blockchain-1.8.0rc1/tests/tools/1315630.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/300000.json` & `chia-blockchain-1.8.0rc1/tests/tools/300000.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/442734.json` & `chia-blockchain-1.8.0rc1/tests/tools/442734.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/466212.json` & `chia-blockchain-1.8.0rc1/tests/tools/466212.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/test-blockchain-db.sqlite` & `chia-blockchain-1.8.0rc1/tests/tools/test-blockchain-db.sqlite`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/test_full_sync.py` & `chia-blockchain-1.8.0rc1/tests/tools/test_full_sync.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/test_legacy_keyring.py` & `chia-blockchain-1.8.0rc1/tests/tools/test_legacy_keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/tools/test_run_block.py` & `chia-blockchain-1.8.0rc1/tests/tools/test_run_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/alert_server.py` & `chia-blockchain-1.8.0rc1/tests/util/alert_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/benchmark_cost.py` & `chia-blockchain-1.8.0rc1/tests/util/benchmark_cost.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/bip39_test_vectors.json` & `chia-blockchain-1.8.0rc1/tests/util/bip39_test_vectors.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/blockchain.py` & `chia-blockchain-1.8.0rc1/tests/util/blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/build_network_protocol_files.py` & `chia-blockchain-1.8.0rc1/tests/util/build_network_protocol_files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/db_connection.py` & `chia-blockchain-1.8.0rc1/tests/util/db_connection.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/gen_ssl_certs.py` & `chia-blockchain-1.8.0rc1/tests/util/gen_ssl_certs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/generator_tools_testing.py` & `chia-blockchain-1.8.0rc1/tests/util/generator_tools_testing.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/key_tool.py` & `chia-blockchain-1.8.0rc1/tests/util/key_tool.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/misc.py` & `chia-blockchain-1.8.0rc1/tests/util/misc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/network_protocol_data.py` & `chia-blockchain-1.8.0rc1/tests/util/network_protocol_data.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/protocol_messages_bytes-v1.0` & `chia-blockchain-1.8.0rc1/tests/util/protocol_messages_bytes-v1.0`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/protocol_messages_json.py` & `chia-blockchain-1.8.0rc1/tests/util/protocol_messages_json.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/rpc.py` & `chia-blockchain-1.8.0rc1/tests/util/rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_chunks.py` & `chia-blockchain-1.8.0rc1/tests/util/test_chunks.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_full_block_utils.py` & `chia-blockchain-1.8.0rc1/tests/util/test_full_block_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_limited_semaphore.py` & `chia-blockchain-1.8.0rc1/tests/util/test_limited_semaphore.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_lock_queue.py` & `chia-blockchain-1.8.0rc1/tests/util/test_lock_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_logging_filter.py` & `chia-blockchain-1.8.0rc1/tests/util/test_logging_filter.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_misc.py` & `chia-blockchain-1.8.0rc1/tests/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_network.py` & `chia-blockchain-1.8.0rc1/tests/util/test_network.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_network_protocol_files.py` & `chia-blockchain-1.8.0rc1/tests/util/test_network_protocol_files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_network_protocol_json.py` & `chia-blockchain-1.8.0rc1/tests/util/test_network_protocol_json.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_network_protocol_test.py` & `chia-blockchain-1.8.0rc1/tests/util/test_network_protocol_test.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_paginator.py` & `chia-blockchain-1.8.0rc1/tests/util/test_paginator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_pprint.py` & `chia-blockchain-1.8.0rc1/tests/util/test_pprint.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_struct_stream.py` & `chia-blockchain-1.8.0rc1/tests/util/test_struct_stream.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/util/test_trusted_peer.py` & `chia-blockchain-1.8.0rc1/tests/util/test_trusted_peer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_lifecycle.py` & `chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_cat_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_outer_puzzle.py` & `chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_cat_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_wallet.py` & `chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_cat_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_offer_lifecycle.py` & `chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_offer_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_trades.py` & `chia-blockchain-1.8.0rc1/tests/wallet/cat_wallet/test_trades.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_db_graftroot.py` & `chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/test_db_graftroot.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from chia.types.coin_spend import CoinSpend
 from chia.types.mempool_inclusion_status import MempoolInclusionStatus
 from chia.types.spend_bundle import SpendBundle
 from chia.util.errors import Err
 from chia.wallet.puzzles.load_clvm import load_clvm
 from chia.wallet.util.merkle_utils import build_merkle_tree, build_merkle_tree_from_binary_tree, simplify_merkle_proof
 
-GRAFTROOT_MOD = load_clvm("graftroot_dl_offers.clvm")
+GRAFTROOT_MOD = load_clvm("graftroot_dl_offers.clsp")
 
 # Always returns the last value
 # (mod solution
 #
 #   (defun recurse (solution last_value)
 #     (if solution
 #         (recurse (r solution) (f solution))
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_offers.py` & `chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/test_dl_offers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_wallet.py` & `chia-blockchain-1.8.0rc1/tests/wallet/db_wallet/test_dl_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/did_wallet/test_did.py` & `chia-blockchain-1.8.0rc1/tests/wallet/did_wallet/test_did.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_1_offers.py` & `chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_1_offers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_bulk_mint.py` & `chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_bulk_mint.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_lifecycle.py` & `chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_offers.py` & `chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_offers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_puzzles.py` & `chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_puzzles.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 )
 from chia.wallet.outer_puzzles import match_puzzle
 from chia.wallet.puzzles.load_clvm import load_clvm
 from chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import puzzle_for_pk, solution_for_conditions
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 from tests.core.make_block_generator import int_to_public_key
 
-SINGLETON_MOD = load_clvm("singleton_top_layer_v1_1.clvm")
-LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clvm")
-DID_MOD = load_clvm("did_innerpuz.clvm")
-NFT_STATE_LAYER_MOD = load_clvm("nft_state_layer.clvm")
-NFT_OWNERSHIP_LAYER = load_clvm("nft_ownership_layer.clvm")
-NFT_TRANSFER_PROGRAM_DEFAULT = load_clvm("nft_ownership_transfer_program_one_way_claim_with_royalties.clvm")
+SINGLETON_MOD = load_clvm("singleton_top_layer_v1_1.clsp")
+LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clsp")
+DID_MOD = load_clvm("did_innerpuz.clsp")
+NFT_STATE_LAYER_MOD = load_clvm("nft_state_layer.clsp")
+NFT_OWNERSHIP_LAYER = load_clvm("nft_ownership_layer.clsp")
+NFT_TRANSFER_PROGRAM_DEFAULT = load_clvm("nft_ownership_transfer_program_one_way_claim_with_royalties.clsp")
 LAUNCHER_PUZZLE_HASH = LAUNCHER_PUZZLE.get_tree_hash()
 NFT_STATE_LAYER_MOD_HASH = NFT_STATE_LAYER_MOD.get_tree_hash()
 SINGLETON_MOD_HASH = SINGLETON_MOD.get_tree_hash()
-OFFER_MOD = load_clvm("settlement_payments.clvm")
+OFFER_MOD = load_clvm("settlement_payments.clsp")
 
 LAUNCHER_ID = Program.to(b"launcher-id").get_tree_hash()
-NFT_METADATA_UPDATER_DEFAULT = load_clvm("nft_metadata_updater_default.clvm")
+NFT_METADATA_UPDATER_DEFAULT = load_clvm("nft_metadata_updater_default.clsp")
 
 
 def test_nft_transfer_puzzle_hashes():
     maker_pk = int_to_public_key(111)
     maker_p2_puz = puzzle_for_pk(maker_pk)
     maker_p2_ph = maker_p2_puz.get_tree_hash()
     maker_did = Program.to("maker did").get_tree_hash()
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_wallet.py` & `chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_nft_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py` & `chia-blockchain-1.8.0rc1/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/rpc/test_dl_wallet_rpc.py` & `chia-blockchain-1.8.0rc1/tests/wallet/rpc/test_dl_wallet_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/rpc/test_wallet_rpc.py` & `chia-blockchain-1.8.0rc1/tests/wallet/rpc/test_wallet_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/simple_sync/test_simple_sync_protocol.py` & `chia-blockchain-1.8.0rc1/tests/wallet/simple_sync/test_simple_sync_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/sync/test_wallet_sync.py` & `chia-blockchain-1.8.0rc1/tests/wallet/sync/test_wallet_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import functools
 import logging
 from typing import List, Optional, Set
 from unittest.mock import MagicMock
 
 import pytest
 from aiosqlite import Error as AIOSqliteError
 from colorlog import getLogger
@@ -1180,19 +1181,25 @@
                     node.coin_state_flaky = False
                     raise PeerRequestException()
                 else:
                     return await func(*args, **kwargs)
 
             return new_func
 
-        def flaky_fetch_puzzle_solution(node, func):
+        request_puzzle_solution_failure_tested = False
+
+        def flaky_request_puzzle_solution(func):
+            @functools.wraps(func)
             async def new_func(*args, **kwargs):
-                if node.puzzle_solution_flaky:
-                    node.puzzle_solution_flaky = False
-                    raise PeerRequestException()
+                nonlocal request_puzzle_solution_failure_tested
+                if not request_puzzle_solution_failure_tested:
+                    request_puzzle_solution_failure_tested = True
+                    # This can just return None if we have `none_response` enabled.
+                    reject = wallet_protocol.RejectPuzzleSolution(bytes32([0] * 32), uint32(0))
+                    return make_msg(ProtocolMessageTypes.reject_puzzle_solution, reject)
                 else:
                     return await func(*args, **kwargs)
 
             return new_func
 
         def flaky_fetch_children(node, func):
             async def new_func(*args, **kwargs):
@@ -1220,26 +1227,25 @@
                     node.db_flaky = False
                     raise AIOSqliteError()
                 else:
                     return await func(*args, **kwargs)
 
             return new_func
 
+        full_node_api.request_puzzle_solution = flaky_request_puzzle_solution(full_node_api.request_puzzle_solution)
+
         for wallet_node, wallet_server in wallets:
             wallet_node.coin_state_retry_seconds = 1
+            request_puzzle_solution_failure_tested = False
             wallet_node.coin_state_flaky = True
-            wallet_node.puzzle_solution_flaky = True
             wallet_node.fetch_children_flaky = True
             wallet_node.get_timestamp_flaky = True
             wallet_node.db_flaky = True
 
             wallet_node.get_coin_state = flaky_get_coin_state(wallet_node, wallet_node.get_coin_state)
-            wallet_node.fetch_puzzle_solution = flaky_fetch_puzzle_solution(
-                wallet_node, wallet_node.fetch_puzzle_solution
-            )
             wallet_node.fetch_children = flaky_fetch_children(wallet_node, wallet_node.fetch_children)
             wallet_node.get_timestamp_for_height = flaky_get_timestamp(
                 wallet_node, wallet_node.get_timestamp_for_height
             )
             wallet_node.wallet_state_manager.puzzle_store.get_wallet_identifier_for_puzzle_hash = (
                 flaky_info_for_puzhash(
                     wallet_node, wallet_node.wallet_state_manager.puzzle_store.get_wallet_identifier_for_puzzle_hash
@@ -1274,15 +1280,15 @@
 
             await time_out_assert(15, tx_in_mempool)
             await full_node_api.farm_new_transaction_block(FarmNewBlockProtocol(bytes32([0] * 32)))
 
             await assert_coin_state_retry()
 
             assert not wallet_node.coin_state_flaky
-            assert not wallet_node.puzzle_solution_flaky
+            assert request_puzzle_solution_failure_tested
             assert not wallet_node.fetch_children_flaky
             assert not wallet_node.get_timestamp_flaky
             assert not wallet_node.db_flaky
             await time_out_assert(30, wallet.get_confirmed_balance, 1_000_000_000_000)
 
     @pytest.mark.asyncio
     async def test_bad_peak_mismatch(self, two_wallet_nodes, default_1000_blocks, self_hostname):
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_address_type.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_address_type.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_bech32m.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_bech32m.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_chialisp.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_chialisp.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_coin_selection.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_coin_selection.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_nft_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_nft_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_notifications.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_notifications.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_offer_parsing_performance.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_offer_parsing_performance.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_puzzle_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_puzzle_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 class TestPuzzleStore:
     @pytest.mark.asyncio
     async def test_puzzle_store(self):
         async with DBConnection(1) as wrapper:
             db = await WalletPuzzleStore.create(wrapper)
             derivation_recs = []
-            # wallet_types = [t for t in WalletType]
-            [t for t in WalletType]
-
             for i in range(1000):
                 derivation_recs.append(
                     DerivationRecord(
                         uint32(i),
                         token_bytes(32),
                         AugSchemeMPL.key_gen(token_bytes(32)).get_g1(),
                         WalletType.STANDARD_WALLET,
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_singleton.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from chia.types.announcement import Announcement
 from chia.types.blockchain_format.program import INFINITE_COST, Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.util.condition_tools import parse_sexp_to_conditions
 from chia.wallet.puzzles.load_clvm import load_clvm
 
-SINGLETON_MOD = load_clvm("singleton_top_layer.clvm")
-LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clvm")
-P2_SINGLETON_MOD = load_clvm("p2_singleton.clvm")
-POOL_MEMBER_MOD = load_clvm("pool_member_innerpuz.clvm")
-POOL_WAITINGROOM_MOD = load_clvm("pool_waitingroom_innerpuz.clvm")
+SINGLETON_MOD = load_clvm("singleton_top_layer.clsp")
+LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clsp")
+P2_SINGLETON_MOD = load_clvm("p2_singleton.clsp")
+POOL_MEMBER_MOD = load_clvm("pool_member_innerpuz.clsp")
+POOL_WAITINGROOM_MOD = load_clvm("pool_waitingroom_innerpuz.clsp")
 
 LAUNCHER_PUZZLE_HASH = LAUNCHER_PUZZLE.get_tree_hash()
 SINGLETON_MOD_HASH = SINGLETON_MOD.get_tree_hash()
 
 LAUNCHER_ID = Program.to(b"launcher-id").get_tree_hash()
 POOL_REWARD_PREFIX_MAINNET = bytes32.fromhex("ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000")
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_singleton_lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from chia.types.coin_spend import CoinSpend
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.types.spend_bundle import SpendBundle
 from chia.util.ints import uint64
 from chia.wallet.puzzles.load_clvm import load_clvm
 from tests.core.full_node.test_conditions import check_spend_bundle_validity, initial_blocks
 
-SINGLETON_MOD = load_clvm("singleton_top_layer.clvm")
-LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clvm")
-P2_SINGLETON_MOD = load_clvm("p2_singleton.clvm")
-POOL_MEMBER_MOD = load_clvm("pool_member_innerpuz.clvm")
-POOL_WAITINGROOM_MOD = load_clvm("pool_waitingroom_innerpuz.clvm")
+SINGLETON_MOD = load_clvm("singleton_top_layer.clsp")
+LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clsp")
+P2_SINGLETON_MOD = load_clvm("p2_singleton.clsp")
+POOL_MEMBER_MOD = load_clvm("pool_member_innerpuz.clsp")
+POOL_WAITINGROOM_MOD = load_clvm("pool_waitingroom_innerpuz.clsp")
 
 LAUNCHER_PUZZLE_HASH = LAUNCHER_PUZZLE.get_tree_hash()
 SINGLETON_MOD_HASH = SINGLETON_MOD.get_tree_hash()
 
 POOL_REWARD_PREFIX_MAINNET = bytes32.fromhex("ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000")
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle_fast.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_singleton_lifecycle_fast.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from chia.types.coin_spend import CoinSpend, compute_additions
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.types.spend_bundle import SpendBundle
 from chia.util.ints import uint64
 from chia.wallet.puzzles.load_clvm import load_clvm
 from tests.clvm.coin_store import BadSpendBundleError, CoinStore, CoinTimestamp
 
-SINGLETON_MOD = load_clvm("singleton_top_layer.clvm")
-LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clvm")
-P2_SINGLETON_MOD = load_clvm("p2_singleton_or_delayed_puzhash.clvm")
-POOL_MEMBER_MOD = load_clvm("pool_member_innerpuz.clvm")
-POOL_WAITINGROOM_MOD = load_clvm("pool_waitingroom_innerpuz.clvm")
+SINGLETON_MOD = load_clvm("singleton_top_layer.clsp")
+LAUNCHER_PUZZLE = load_clvm("singleton_launcher.clsp")
+P2_SINGLETON_MOD = load_clvm("p2_singleton_or_delayed_puzhash.clsp")
+POOL_MEMBER_MOD = load_clvm("pool_member_innerpuz.clsp")
+POOL_WAITINGROOM_MOD = load_clvm("pool_waitingroom_innerpuz.clsp")
 
 LAUNCHER_PUZZLE_HASH = LAUNCHER_PUZZLE.get_tree_hash()
 SINGLETON_MOD_HASH = SINGLETON_MOD.get_tree_hash()
 P2_SINGLETON_MOD_HASH = P2_SINGLETON_MOD.get_tree_hash()
 
 ANYONE_CAN_SPEND_PUZZLE = Program.to(1)
 ANYONE_CAN_SPEND_WITH_PADDING_PUZZLE_HASH = Program.to(binutils.assemble("(a (q . 1) 3)")).get_tree_hash()
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_taproot.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_taproot.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_transaction_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_transaction_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import dataclasses
 from secrets import token_bytes
-from typing import Any, List
+from typing import Any, List, Optional, Tuple
 
 import pytest
 
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.mempool_inclusion_status import MempoolInclusionStatus
 from chia.util.errors import Err
 from chia.util.ints import uint8, uint32, uint64
-from chia.wallet.transaction_record import TransactionRecord
+from chia.wallet.transaction_record import TransactionRecord, minimum_send_attempts
 from chia.wallet.util.transaction_type import TransactionType
 from chia.wallet.wallet_transaction_store import WalletTransactionStore, filter_ok_mempool_status
 from tests.util.db_connection import DBConnection
 
 coin_1 = Coin(token_bytes(32), token_bytes(32), uint64(12312))
 coin_2 = Coin(token_bytes(32), token_bytes(32), uint64(1234))
 coin_3 = Coin(token_bytes(32), token_bytes(32), uint64(12312 - 1234))
@@ -648,7 +648,30 @@
         assert cmp(not_sent, [tr1, tr3, tr4])
 
         # the 6th time we call this function, we don't get any unsent txs
         not_sent = await store.get_not_sent()
         assert cmp(not_sent, [])
 
         # TODO: also cover include_accepted_txs=True
+
+
+@pytest.mark.asyncio
+async def test_transaction_record_is_valid() -> None:
+    invalid_attempts: List[Tuple[str, uint8, Optional[str]]] = []
+    # The tx should be valid as long as we don't have minimum_send_attempts failed attempts
+    while len(invalid_attempts) < minimum_send_attempts:
+        assert dataclasses.replace(tr1, sent_to=invalid_attempts).is_valid()
+        invalid_attempts.append(("peer", uint8(MempoolInclusionStatus.FAILED), None))
+    # The tx should be invalid now with more than minimum failed attempts
+    assert len(invalid_attempts) == minimum_send_attempts
+    assert not dataclasses.replace(tr1, sent_to=invalid_attempts).is_valid()
+    mempool_success = ("success", uint8(MempoolInclusionStatus.SUCCESS), None)
+    low_fee = ("low_fee", uint8(MempoolInclusionStatus.FAILED), Err.INVALID_FEE_LOW_FEE.name)
+    close_to_zero = (
+        "close_to_zero",
+        uint8(MempoolInclusionStatus.FAILED),
+        Err.INVALID_FEE_TOO_CLOSE_TO_ZERO.name,
+    )
+    # But it should become valid with one of the above attempts
+    assert dataclasses.replace(tr1, sent_to=invalid_attempts + [mempool_success]).is_valid()
+    assert dataclasses.replace(tr1, sent_to=invalid_attempts + [low_fee]).is_valid()
+    assert dataclasses.replace(tr1, sent_to=invalid_attempts + [close_to_zero]).is_valid()
```

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_blockchain.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_coin_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_interested_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_interested_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_key_val_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_key_val_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_node.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_node.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_retry.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_retry.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_state_manager.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_state_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_trade_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_trade_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_user_store.py` & `chia-blockchain-1.8.0rc1/tests/wallet/test_wallet_user_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tests/weight_proof/test_weight_proof.py` & `chia-blockchain-1.8.0rc1/tests/weight_proof/test_weight_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/analyze-chain.py` & `chia-blockchain-1.8.0rc1/tools/analyze-chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,52 +3,42 @@
 from __future__ import annotations
 
 import sqlite3
 import sys
 from functools import partial
 from pathlib import Path
 from time import time
-from typing import Callable, List, Optional, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import click
 import zstd
 from blspy import AugSchemeMPL, G1Element
-from chia_rs import MEMPOOL_MODE, run_generator
+from chia_rs import MEMPOOL_MODE, SpendBundleConditions, run_block_generator
 
 from chia.consensus.default_constants import DEFAULT_CONSTANTS
 from chia.types.block_protocol import BlockInfo
-from chia.types.blockchain_format.program import Program
+from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.blockchain_format.sized_bytes import bytes32, bytes48
 from chia.types.full_block import FullBlock
 from chia.util.condition_tools import pkm_pairs
 from chia.util.full_block_utils import block_info_from_block, generator_from_block
-from chia.wallet.puzzles.rom_bootstrap_generator import get_generator
 
-GENERATOR_ROM = bytes(get_generator())
 
-
-# returns an optional error code and an optional PySpendBundleConditions (from chia_rs)
+# returns an optional error code and an optional SpendBundleConditions (from chia_rs)
 # exactly one of those will hold a value and the number of seconds it took to
 # run
-def run_gen(env_data: bytes, block_program_args: bytes, flags: int):
-    max_cost = DEFAULT_CONSTANTS.MAX_BLOCK_COST_CLVM
-    cost_per_byte = DEFAULT_CONSTANTS.COST_PER_BYTE
-
-    # we don't charge for the size of the generator ROM. However, we do charge
-    # cost for the operations it executes
-    max_cost -= len(env_data) * cost_per_byte
-
-    env_data = b"\xff" + env_data + b"\xff" + block_program_args + b"\x80"
-
+def run_gen(
+    generator_program: SerializedProgram, block_program_args: List[bytes], flags: int
+) -> Tuple[Optional[int], Optional[SpendBundleConditions], float]:
     try:
         start_time = time()
-        err, result = run_generator(
-            GENERATOR_ROM,
-            env_data,
-            max_cost,
+        err, result = run_block_generator(
+            bytes(generator_program),
+            block_program_args,
+            DEFAULT_CONSTANTS.MAX_BLOCK_COST_CLVM,
             flags,
         )
         run_time = time() - start_time
         return err, result, run_time
     except Exception as e:
         # GENERATOR_RUNTIME_ERROR
         sys.stderr.write(f"Exception: {e}\n")
@@ -127,25 +117,20 @@
     generator_blobs: List[bytes],
     ref_lookup_time: float,
     flags: int,
 ) -> None:
     num_refs = len(generator_blobs)
 
     # add the block program arguments
-    block_program_args = bytearray(b"\xff")
-    for ref_block_blob in generator_blobs:
-        block_program_args += b"\xff"
-        block_program_args += Program.to(ref_block_blob).as_bin()
-    block_program_args += b"\x80\x80"
-
     assert block.transactions_generator is not None
-    err, result, run_time = run_gen(bytes(block.transactions_generator), bytes(block_program_args), flags)
+    err, result, run_time = run_gen(block.transactions_generator, generator_blobs, flags)
     if err is not None:
         sys.stderr.write(f"ERROR: {hh.hex()} {height} {err}\n")
         return
+    assert result is not None
 
     num_removals = len(result.spends)
     fees = result.reserve_fee
     cost = result.cost
     num_additions = 0
     for spends in result.spends:
         num_additions += len(spends.create_coin)
```

### Comparing `chia-blockchain-1.8.0b6/tools/analyze_memory_profile.py` & `chia-blockchain-1.8.0rc1/tools/analyze_memory_profile.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/cpu_utilization.py` & `chia-blockchain-1.8.0rc1/tools/cpu_utilization.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/generate_chain.py` & `chia-blockchain-1.8.0rc1/tools/generate_chain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/legacy_keyring.py` & `chia-blockchain-1.8.0rc1/tools/legacy_keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/plot-log.gnuplot` & `chia-blockchain-1.8.0rc1/tools/plot-log.gnuplot`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/run_benchmark.sh` & `chia-blockchain-1.8.0rc1/tools/run_benchmark.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/run_block.py` & `chia-blockchain-1.8.0rc1/tools/run_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 from chia.util.default_root import DEFAULT_ROOT_PATH
 from chia.util.ints import uint32, uint64
 from chia.wallet.cat_wallet.cat_utils import match_cat_puzzle
 from chia.wallet.puzzles.load_clvm import load_serialized_clvm_maybe_recompile
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 
 DESERIALIZE_MOD = load_serialized_clvm_maybe_recompile(
-    "chialisp_deserialisation.clvm", package_or_requirement="chia.wallet.puzzles"
+    "chialisp_deserialisation.clsp", package_or_requirement="chia.wallet.puzzles"
 )
 
 
 @dataclass
 class NPC:
     coin_name: bytes32
     puzzle_hash: bytes32
```

### Comparing `chia-blockchain-1.8.0b6/tools/test_constants.py` & `chia-blockchain-1.8.0rc1/tools/test_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b6/tools/test_full_sync.py` & `chia-blockchain-1.8.0rc1/tools/test_full_sync.py`

 * *Files identical despite different names*

