# Comparing `tmp/scikit_build_core-0.3.1.tar.gz` & `tmp/scikit_build_core-0.3.2.tar.gz`

## Comparing `scikit_build_core-0.3.1.tar` & `scikit_build_core-0.3.2.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.gitattributes
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.packit.yaml
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.readthedocs.yml
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/noxfile.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.distro/scikit-build-core.spec
--rw-r--r--   0        0        0     8835 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/changelog.md
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/conf.py
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/configuration.md
--rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/setuptools/extension.py
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/constraints.txt
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_cmake_config.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_fileapi.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_generator_default.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_get_requires.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_program_search.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_settings.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_simple_pure.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_simplest_c.py
--rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/LICENSE
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/README.md
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.gitattributes
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.packit.yaml
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.readthedocs.yml
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/noxfile.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.distro/scikit-build-core.spec
+-rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/changelog.md
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/conf.py
+-rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/configuration.md
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/setuptools/extension.py
+-rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_fileapi.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_get_requires.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/LICENSE
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/README.md
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/PKG-INFO
```

### Comparing `scikit_build_core-0.3.1/.packit.yaml` & `scikit_build_core-0.3.2/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/.pre-commit-config.yaml` & `scikit_build_core-0.3.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
           - rich
           - setuptools-scm
           - tomli
           - types-setuptools>=67.6.0.5
           - typing_extensions>=4;python_version<'3.11'
 
   - repo: https://github.com/henryiii/check-sdist
-    rev: "v0.1.0"
+    rev: "v0.1.1"
     hooks:
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
           - hatchling
           - hatch-vcs
```

### Comparing `scikit_build_core-0.3.1/noxfile.py` & `scikit_build_core-0.3.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/.distro/scikit-build-core.spec` & `scikit_build_core-0.3.2/.distro/scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/.github/CONTRIBUTING.md` & `scikit_build_core-0.3.2/.github/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -284,14 +284,36 @@
 from scikit_build_core.setuptoools.extension import CMakeExtension
 ...
 cmake_extensions=[CMakeExtension("cmake_example")],
 ```
 
 Which should eventually support multiple extensions.
 
+## Patterns
+
+### Backports
+
+All backported standard library code is in `scikit_build_core._compat`, in a
+module with the stdlib name.
+
+### Detecting the platform
+
+Here are some common platforms and the reported values:
+
+| OS      | Compiler   | `sys.platform` | `sysconfig.get_platform()`   |
+| ------- | ---------- | -------------- | ---------------------------- |
+| Windows | MSVC       | `win32`        | `win-amd64`                  |
+| Windows | MinGW      | `win32`        | `mingw_x86_64`               |
+| Windows | MinGW URCT | `win32`        | `mingw_x86_64_ucrt`          |
+| Windows | Cygwin     | `cygwin`       | `cygwin-3.4.6-x86_64`        |
+| macOS   | Clang      | `darwin`       | `macosx-10.15-x86_64`        |
+| Linux   | GCC        | `linux`        | `linux-x86_64`               |
+| Pyodide | Clang      | `emscripten`   | `emscripten-3.1.32-wasm32`   |
+| FreeBSD | GCC        | `freebsd13`    | `freebsd-13.2-RELEASE-amd64` |
+
 # Downstream packaging
 
 ## Fedora packaging
 
 We are using [`packit`](https://packit.dev/) to keep maintain the
 [Fedora package](https://src.fedoraproject.org/rpms/python-scikit-build-core/).
 There are two `packit` jobs one needs to keep in mind here:
```

### Comparing `scikit_build_core-0.3.1/.github/matchers/pylint.json` & `scikit_build_core-0.3.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/.github/workflows/cd.yml` & `scikit_build_core-0.3.2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/.github/workflows/ci.yml` & `scikit_build_core-0.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/changelog.md` & `scikit_build_core-0.3.2/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## Version 0.3.2
+
+Some small fixes for edge cases. Several docs improvements, too.
+
+Fixes:
+
+- Suppress Unicode errors in scripts dir and move on by @henryiii in #294
+- Specify platform properly for non-MSVC Windows by @henryiii in #295
+
+Docs:
+
+- Doc updates by @zerothi in #287
+- Add a bit to plugin instructions by @henryiii in #289
+- Typos fixed by @afh in #291 and #292
+
 ## Version 0.3.1
 
 This is a small release fixing a regression in some cases caused by adding
 `Python_LIBRARY`. This has been reverted on non-Windows platforms, since it is
 only needed on Windows.
 
 ### What's Changed
```

### Comparing `scikit_build_core-0.3.1/docs/cmakelists.md` & `scikit_build_core-0.3.2/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/conf.py` & `scikit_build_core-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/configuration.md` & `scikit_build_core-0.3.2/docs/configuration.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,30 +120,30 @@
 [tool.scikit-build]
 backport.find-python = "3.15"
 ```
 
 ## Configuring source file inclusion
 
 Scikit-build-core defaults to using your `.gitignore` to select what to exclude
-from the wheel. You can list files to explicitly include and exclude if you
-want:
+from the source distribution. You can list files to explicitly include and
+exclude if you want:
 
 ```toml
 [tool.scikit-build]
-sdist.include = ["src/some_geneerated_file.txt"]
+sdist.include = ["src/some_generated_file.txt"]
 sdist.exclude = [".github"]
 ```
 
 By default, scikit-build-core will respect `SOURCE_DATE_EPOCH`, and will lock
 the modification time to a reproducible value if it's not set. You can disable
 reproducible builds if you prefer, however:
 
 ```toml
 [tool.scikit-build]
-sdist.reproducible = true
+sdist.reproducible = false
 ```
 
 ## Customizing the built wheel
 
 The wheel will automatically look for Python packages at `<package_name>` and
 `src/<package_name>`. If you want to list packages explicitly, you can:
 
@@ -370,15 +370,15 @@
 
 ````
 
 ## Dynamic metadata (WIP)
 
 Scikit-build-core 0.3.0 will support dynamic metadata. This is not ready for
 plugin development outside of scikit-build-core;
-`tool.scikit-build.expiremental=true` is required to use external plugins, since
+`tool.scikit-build.experimental=true` is required to use external plugins, since
 the interface is provisional. Nested arbitrary dicts (as seen here) are not
 supported in config-settings or environment variables.
 
 There currently are two built-in plugins for dynamic metadata.
 
 :::{tab} Setuptools-scm
 
@@ -388,14 +388,18 @@
 ```toml
 [project]
 name = "mypackage"
 dynamic = ["version"]
 
 [tool.scikit-build]
 metadata.version.provider = "scikit_build_core.metadata.setuptools_scm"
+sdist.include = ["src/package/_version.py"]
+
+[tool.setuptools_scm]
+write_to = "src/package/_version.py"
 ```
 
 This sets the python project version according to
 [git tags](https://github.com/pypa/setuptools_scm/blob/fb261332d9b46aa5a258042d85baa5aa7b9f4fa2/README.rst#default-versioning-scheme)
 or a
 [`.git_archival.txt`](https://github.com/pypa/setuptools_scm/blob/fb261332d9b46aa5a258042d85baa5aa7b9f4fa2/README.rst#git-archives)
 file, or equivalents for other VCS systems. With this, you may also to set the
@@ -425,14 +429,16 @@
 ```toml
 [project]
 name = "mypackage"
 dynamic = ["readme"]
 
 [tool.scikit-build]
 metadata.readme.provider = "scikit_build_core.metadata.fancy_pypi_readme"
+
+# tool.hatch.metadata.hooks.fancy-pypi-readme options here
 ```
 
 :::
 
 ## Editable installs
 
 Experimental support for editable installs is provided, with some caveats and
@@ -447,15 +453,15 @@
 - You need to reinstall to pick up new files.
 
 Known limitations:
 
 - Resources (via `importlib.resources`) are not properly supported (yet).
 
 ```console
-# Very expiremental rebuild on initial import feature
+# Very experimental rebuild on initial import feature
 $ pip install --no-build-isolation --config-settings=editiable.rebuild=true -ve.
 ```
 
 Due to the length of this line already being long, you do not need to set the
 `experimental` setting to use editable installs, but please consider them
 experimental and subject to change.
```

### Comparing `scikit_build_core-0.3.1/docs/getting_started.md` & `scikit_build_core-0.3.2/docs/getting_started.md`

 * *Files 0% similar despite different names*

```diff
@@ -74,17 +74,16 @@
 └── CMakeLists.txt
 ```
 
 ````
 
 ### Source code
 
-For this tutorial, you can either use write a C extension yourself, or you can
-use pybind11 and C++. Select your preferred version using the tabs - compare
-them!
+For this tutorial, you can either write a C extension yourself, or you can use
+pybind11 and C++. Select your preferred version using the tabs - compare them!
 
 ````{tab} C
 
 ```{literalinclude} examples/getting_started/c/example.c
 :language: c
 ```
```

### Comparing `scikit_build_core-0.3.1/docs/index.md` & `scikit_build_core-0.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.3.2/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.3.2/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.3.2/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.3.2/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.3.2/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.3.2/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/_logging.py` & `scikit_build_core-0.3.2/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.3.2/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/cmake.py` & `scikit_build_core-0.3.2/src/scikit_build_core/cmake.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import contextlib
 import dataclasses
 import json
 import os
 import shutil
 import subprocess
 import sys
+import sysconfig
 import textwrap
 from collections.abc import Mapping, Sequence
 from pathlib import Path
 from typing import Generator
 
 from packaging.version import Version
 
@@ -62,15 +63,15 @@
     source_dir: Path
     build_dir: Path
     build_type: str
     module_dirs: list[Path] = dataclasses.field(default_factory=list)
     prefix_dirs: list[Path] = dataclasses.field(default_factory=list)
     init_cache_file: Path = dataclasses.field(init=False, default=Path())
     env: dict[str, str] = dataclasses.field(init=False, default_factory=os.environ.copy)
-    single_config: bool = not sys.platform.startswith("win32")
+    single_config: bool = not sysconfig.get_platform().startswith("win")
 
     def __post_init__(self) -> None:
         self.init_cache_file = self.build_dir / "CMakeInit.txt"
 
         if not self.source_dir.is_dir():
             msg = f"source directory {self.source_dir} does not exist"
             raise CMakeConfigError(msg)
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/errors.py` & `scikit_build_core-0.3.2/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/program_search.py` & `scikit_build_core-0.3.2/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.3.2/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/_scripts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import contextlib
 import re
 from pathlib import Path
 
 __all__ = ["process_script_dir"]
 
 
 def __dir__() -> list[str]:
@@ -12,15 +13,15 @@
 
 SHEBANG_PATTERN = re.compile(r"^#!.*(?:python|pythonw|pypy)[0-9.]*([ \t].*)?$")
 
 
 def process_script_dir(script_dir: Path) -> None:
     for item in script_dir.iterdir():
         content = []
-        with item.open(encoding="utf-8") as f:
+        with contextlib.suppress(UnicodeDecodeError), item.open(encoding="utf-8") as f:
             file_iter = iter(f)
             try:
                 # TODO: handle empty files
                 first_line = next(file_iter)
             except StopIteration:
                 first_line = ""
             match = SHEBANG_PATTERN.match(first_line)
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.3.2/src/scikit_build_core/build/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import os
 import shutil
 import sys
+import sysconfig
 import tempfile
 from collections.abc import Sequence
 from pathlib import Path
 
 from packaging.version import Version
 
 from .. import __version__
@@ -176,15 +177,16 @@
             defines=defines,
             cache_entries=cache_entries,
             name=metadata.name,
             version=metadata.version,
         )
 
         generator = builder.config.env.get(
-            "CMAKE_GENERATOR", "MSVC" if sys.platform.startswith("win32") else "Unknown"
+            "CMAKE_GENERATOR",
+            "MSVC" if sysconfig.get_platform().startswith("win") else "Unknown",
         )
         rich_print(
             f"[green]***[/green] [bold]Building project with [blue]{generator}[/blue]..."
         )
         build_args: list[str] = []
         builder.build(build_args=build_args)
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.3.2/src/scikit_build_core/builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import re
 import sys
 import sysconfig
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 from pathlib import Path
-from typing import Mapping
 
 from packaging.version import Version
 
 from .. import __version__
 from .._compat.importlib import metadata, resources
 from .._logging import logger
 from ..cmake import CMaker
@@ -141,20 +140,20 @@
         # Modern Find Python
         for prefix in ("Python", "Python3"):
             cache_config[f"{prefix}_EXECUTABLE"] = sys.executable
             cache_config[f"{prefix}_ROOT_DIR"] = sys.prefix
             cache_config[f"{prefix}_INCLUDE_DIR"] = python_include_dir
             cache_config[f"{prefix}_FIND_REGISTRY"] = "NEVER"
             # FindPython may break if this is set - only useful on Windows
-            if python_library and sys.platform.startswith("win"):
+            if python_library and sysconfig.get_platform().startswith("win"):
                 cache_config[f"{prefix}_LIBRARY"] = python_library
 
         if limited_abi:
             cache_config["SKBUILD_SOABI"] = (
-                "" if sys.platform.startswith("win") else "abi3"
+                "" if sysconfig.get_platform().startswith("win") else "abi3"
             )
         else:
             # Workaround for bug in PyPy and packaging that is not handled in CMake
             # According to PEP 3149, SOABI and EXT_SUFFIX are interchangeable (and
             # the latter is much more likely to be correct as it is used elsewhere)
             if sys.version_info < (3, 8, 7):
                 # See https://github.com/python/cpython/issues/84006
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.3.2/src/scikit_build_core/builder/generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import re
 import subprocess
 import sys
+import sysconfig
 from collections.abc import Mapping, MutableMapping
 
 from packaging.version import Version
 
 from .._logging import logger
 from ..cmake import CMake
 from ..errors import NinjaNotFoundError
@@ -63,22 +64,28 @@
     have one set; if ninja is present, ninja will be used over make on Unix.
     """
 
     default = get_default(cmake) or ""
     if default:
         logger.debug("Default generator: {}", default)
 
-    if sys.platform.startswith("win32") and "Visual Studio" in env.get(
+    if sysconfig.get_platform().startswith("win") and "Visual Studio" in env.get(
         "CMAKE_GENERATOR", default
     ):
         # This must also be set when *_PLATFORM is set.
         env.setdefault("CMAKE_GENERATOR", default)
         env.setdefault("CMAKE_GENERATOR_PLATFORM", get_cmake_platform(env))
         return {}
 
+    if sys.platform.startswith("win") and not sysconfig.get_platform().startswith(
+        "win"
+    ):
+        # Non-MSVC Windows platforms require Ninja
+        env.setdefault("CMAKE_GENERATOR", "Ninja")
+
     if env.get("CMAKE_GENERATOR", default or "Ninja") == "Ninja":
         min_ninja = Version(ninja_settings.minimum_version)
         ninja = best_program(get_ninja_programs(), minimum_version=min_ninja)
 
         if ninja is not None:
             env.setdefault("CMAKE_GENERATOR", "Ninja")
             logger.debug("CMAKE_GENERATOR: Using ninja: {}", ninja.path)
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.3.2/src/scikit_build_core/builder/get_requires.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import functools
 import os
-import sys
+import sysconfig
 from collections.abc import Generator, Mapping
 
 from packaging.tags import sys_tags
 from packaging.version import Version
 
 from .._compat import tomllib
 from .._compat.typing import Literal
@@ -56,16 +56,16 @@
         )
         if cmake is None:
             yield f"cmake>={cmake_min}"
             return
         logger.debug("Found system CMake: {} - not requiring PyPI package", cmake)
 
     def ninja(self) -> Generator[str, None, None]:
-        # On Windows, Ninja is not default
-        if sys.platform.startswith("win") and "Ninja" not in os.environ.get(
+        # On Windows MSVC, Ninja is not default
+        if sysconfig.get_platform().startswith("win") and "Ninja" not in os.environ.get(
             "CMAKE_GENERATOR", ""
         ):
             return
 
         # If something besides Windows is set, don't add ninja
         if "Ninja" not in os.environ.get("CMAKE_GENERATOR", "Ninja"):
             return
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.3.2/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.3.2/src/scikit_build_core/builder/sysconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 def get_platform(env: Mapping[str, str] | None = None) -> str:
     """
     Return the Python platform name for a platform, respecting VSCMD_ARG_TGT_ARCH.
     """
     if env is None:
         env = os.environ
-    if sys.platform.startswith("win"):
+    if sysconfig.get_platform().startswith("win"):
         if "VSCMD_ARG_TGT_ARCH" in env:
             logger.debug(
                 "Selecting {} or {} due to VSCMD_ARG_TARGET_ARCH",
                 TARGET_TO_PLAT.get(env["VSCMD_ARG_TGT_ARCH"]),
                 get_host_platform(),
             )
             return TARGET_TO_PLAT.get(env["VSCMD_ARG_TGT_ARCH"]) or get_host_platform()
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.3.2/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.3.2/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=duplicate-code
 
 import builtins
 import json
 from pathlib import Path
-from typing import Any, Callable, Dict, Type, TypeVar
+from typing import Any, Callable, Dict, Type, TypeVar  # noqa: TID251
 
 import cattr
 import cattr.preconf.json
 
 from .model.cache import Cache
 from .model.cmakefiles import CMakeFiles
 from .model.codemodel import CodeModel, Target
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.3.2/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.3.2/src/scikit_build_core/file_api/reply.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import builtins
 import dataclasses
 import json
 import sys
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Type, TypeVar, Union
+from typing import Any, Callable, Dict, List, Type, TypeVar, Union  # noqa: TID251
 
 from .._compat.builtins import ExceptionGroup
 from .model.cache import Cache
 from .model.cmakefiles import CMakeFiles
 from .model.codemodel import CodeModel, Target
 from .model.directory import Directory
 from .model.index import Index
```

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.3.2/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.3.2/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.3.2/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.3.2/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.3.2/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.3.2/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/src/scikit_build_core/setuptools/extension.py` & `scikit_build_core-0.3.2/src/scikit_build_core/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/conftest.py` & `scikit_build_core-0.3.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import contextlib
 import dataclasses
 import importlib.util
 import os
 import shutil
 import subprocess
 import sys
+import sysconfig
 import types
 import warnings
 from collections.abc import Generator
 from pathlib import Path
 from venv import EnvBuilder
 
 if sys.version_info < (3, 8):
@@ -292,8 +293,12 @@
         "wheel",
     ]
     valid = []
     for package in interesting_packages:
         with contextlib.suppress(ModuleNotFoundError):
             valid.append(f"{package}=={metadata.version(package)}")  # type: ignore[no-untyped-call]
     reqs = " ".join(valid)
-    return f"installed packages of interest: {reqs}"
+    lines = [
+        f"installed packages of interest: {reqs}",
+        f"sysconfig platform: {sysconfig.get_platform()}",
+    ]
+    return "\n".join(lines)
```

### Comparing `scikit_build_core-0.3.1/tests/test_builder.py` & `scikit_build_core-0.3.2/tests/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 @pytest.mark.xfail(
     strict=False, reason="Doesn't matter if this fails, usually not used"
 )
 def test_get_python_library():
     pprint.pprint(sysconfig.get_config_vars())
 
     lib = get_python_library({})
-    if sys.platform.startswith("win"):
-        assert lib is None
-    else:
+    if sysconfig.get_platform().startswith("win"):
         assert lib
         assert lib.is_file()
+    else:
+        assert lib is None
 
 
-@pytest.mark.skipif(not sys.platform.startswith("win"), reason="Windows only")
+@pytest.mark.skipif(not sysconfig.get_platform().startswith("win"), reason="MSVC only")
 def test_get_python_library_xcompile(tmp_path):
     config_path = tmp_path / "tmp.cfg"
     config_path.write_text(
         """\
 [build_ext]
 library_dirs=C:\\Python\\libs
     """
```

### Comparing `scikit_build_core-0.3.1/tests/test_cmake_config.py` & `scikit_build_core-0.3.2/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_dynamic_metadata.py` & `scikit_build_core-0.3.2/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_fileapi.py` & `scikit_build_core-0.3.2/tests/test_fileapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import shutil
-import sys
+import sysconfig
 from pathlib import Path
 
 import pytest
 from packaging.version import Version
 
 from scikit_build_core.cmake import CMake, CMaker
 from scikit_build_core.file_api._cattrs_converter import (
@@ -20,15 +20,15 @@
 has_make = shutil.which("make") is not None or shutil.which("gmake") is not None
 has_ninja = shutil.which("ninja") is not None
 
 
 def prepare_env_or_skip() -> None:
     if (
         "CMAKE_GENERATOR" not in os.environ
-        and not sys.platform.startswith("win32")
+        and not sysconfig.get_platform().startswith("win")
         and not has_make
     ):
         if has_ninja:
             os.environ["CMAKE_GENERATOR"] = "Ninja"
         else:
             pytest.skip("No build system found")
```

### Comparing `scikit_build_core-0.3.1/tests/test_fortran.py` & `scikit_build_core-0.3.2/tests/test_fortran.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,16 @@
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.fortran()
 @pytest.mark.skipif(shutil.which("gfortran") is None, reason="gfortran not available")
 @pytest.mark.skipif(
-    sysconfig.get_platform().startswith("msys"),
-    reason="Fortran not working with MSYS yet",
-)
-@pytest.mark.skipif(
-    sys.platform.startswith("win"),
-    reason="No reasonable Fortran compiler available on Windows",
+    sysconfig.get_platform().startswith("win"),
+    reason="No reasonable Fortran compiler for MSVC",
 )
 def test_pep517_wheel(tmp_path, monkeypatch, virtualenv):
     dist = tmp_path / "dist"
     dist.mkdir()
     monkeypatch.chdir(FORTRAN_EXAMPLE)
     if Path("dist").is_dir():
         shutil.rmtree("dist")
```

### Comparing `scikit_build_core-0.3.1/tests/test_generator_default.py` & `scikit_build_core-0.3.2/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_get_requires.py` & `scikit_build_core-0.3.2/tests/test_get_requires.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import shutil
 import sys
+import sysconfig
 from pathlib import Path
 
 import pytest
 
 from scikit_build_core.build import (
     get_requires_for_build_editable,
     get_requires_for_build_sdist,
     get_requires_for_build_wheel,
 )
 from scikit_build_core.builder.get_requires import GetRequires
 
-ninja = [] if sys.platform.startswith("win") else ["ninja>=1.5"]
+ninja = [] if sysconfig.get_platform().startswith("win") else ["ninja>=1.5"]
 
 
 def which_mock(name: str) -> str | None:
     if name in ("ninja", "ninja-build", "cmake3", "samu", "gmake", "make"):
         return None
     if name == "cmake":
         return "cmake/path"
```

### Comparing `scikit_build_core-0.3.1/tests/test_module_dir.py` & `scikit_build_core-0.3.2/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_name_main.py` & `scikit_build_core-0.3.2/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_prepare_metadata.py` & `scikit_build_core-0.3.2/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_process_scripts.py` & `scikit_build_core-0.3.2/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_program_search.py` & `scikit_build_core-0.3.2/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_pyproject_abi3.py` & `scikit_build_core-0.3.2/tests/test_pyproject_abi3.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.skipif(
     sys.implementation.name == "pypy", reason="pypy does not support abi3"
 )
 @pytest.mark.skipif(
-    SYSCONFIGPLAT.startswith(("msys", "mingw")),
+    sysconfig.get_platform().startswith(("msys", "mingw")),
     reason="abi3 FindPython on MSYS/MinGW reports not found",
 )
 def test_abi3_wheel(tmp_path, monkeypatch, virtualenv):
     dist = tmp_path / "dist"
     dist.mkdir()
     monkeypatch.chdir(ABI_PKG)
     if Path("dist").is_dir():
@@ -42,15 +42,15 @@
             file_names = [p.name for p in p.iterdir()]
 
         assert len(file_names) == 2
         assert "abi3_example-0.0.1.dist-info" in file_names
         file_names.remove("abi3_example-0.0.1.dist-info")
         (so_file,) = file_names
 
-        if sys.platform.startswith("win"):
+        if sysconfig.get_platform().startswith("win"):
             assert so_file == "abi3_example.pyd"
         elif sys.platform.startswith("cygwin"):
             assert so_file == "abi3_example.abi3.dll"
         else:
             assert so_file == "abi3_example.abi3.so"
 
     virtualenv.install(wheel)
```

### Comparing `scikit_build_core-0.3.1/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.3.2/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_pyproject_pep517.py` & `scikit_build_core-0.3.2/tests/test_pyproject_pep517.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 Version: 0.0.1
 Requires-Python: >=3.7
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 """
 
 mark_hashes_different = pytest.mark.xfail(
-    sys.platform.startswith("win32") or sys.platform.startswith("cygwin"),
+    sys.platform.startswith(("win", "cygwin")),
     reason="hashes differ on Windows",
     strict=False,
 )
 
 
 @pytest.mark.usefixtures("package_simple_pyproject_ext")
 def test_pep517_sdist():
```

### Comparing `scikit_build_core-0.3.1/tests/test_pyproject_pep518.py` & `scikit_build_core-0.3.2/tests/test_pyproject_pep518.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """
     )
 
     subprocess.run([sys.executable, "-m", "build", "--sdist"], check=True)
     (sdist,) = Path("dist").iterdir()
     assert sdist.name == "cmake-example-0.0.1.tar.gz"
 
-    if not (sys.platform.startswith("win32") or sys.platform.startswith("cygwin")):
+    if not sys.platform.startswith(("win", "cygwin")):
         hash = hashlib.sha256(sdist.read_bytes()).hexdigest()
         assert hash == package_simple_pyproject_ext.sdist_hash
 
     with tarfile.open(sdist) as f:
         file_names = set(f.getnames())
         assert file_names == {
             f"cmake-example-0.0.1/{x}"
```

### Comparing `scikit_build_core-0.3.1/tests/test_pyproject_pep660.py` & `scikit_build_core-0.3.2/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_settings.py` & `scikit_build_core-0.3.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_setuptools_abi3.py` & `scikit_build_core-0.3.2/tests/test_setuptools_abi3.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     assert virtualenv.execute("print('hello')") == "hello"
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = {p.name for p in p.iterdir()}
 
-        if sys.platform.startswith("win"):
+        if sysconfig.get_platform().startswith("win"):
             assert "abi3_example.pyd" in file_names
         elif sys.platform.startswith("cygwin"):
             assert "abi3_example.abi3.dll" in file_names
         else:
             assert "abi3_example.abi3.so" in file_names
 
     virtualenv.install(wheel)
```

### Comparing `scikit_build_core-0.3.1/tests/test_setuptools_pep517.py` & `scikit_build_core-0.3.2/tests/test_setuptools_pep517.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,18 @@
         assert metadata_set <= pkg_info_contents
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.broken_on_urct()
 @pytest.mark.usefixtures("package_simple_setuptools_ext")
-@pytest.mark.skipif(
-    sys.platform.startswith("cygwin"), reason="Cygwin fails here with ld errors"
+@pytest.mark.xfail(
+    sys.platform.startswith("cygwin"),
+    reason="Cygwin fails here with ld errors",
+    strict=False,
 )
 def test_pep517_wheel(virtualenv):
     dist = Path("dist")
     out = build_wheel("dist")
     (wheel,) = dist.glob("cmake_example-0.0.1-*.whl")
     assert wheel == dist / out
```

### Comparing `scikit_build_core-0.3.1/tests/test_setuptools_pep518.py` & `scikit_build_core-0.3.2/tests/test_setuptools_pep518.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 
 
 # TODO: work out why this fails on Cygwin
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
 @pytest.mark.broken_on_urct()
-@pytest.mark.skipif(
-    sys.platform.startswith("cygwin"), reason="Cygwin fails here with ld errors"
+@pytest.mark.xfail(
+    sys.platform.startswith("cygwin"),
+    reason="Cygwin fails here with ld errors",
+    strict=False,
 )
 @pytest.mark.usefixtures("package_simple_setuptools_ext")
 def test_pep518_wheel(isolated):
     dist = Path("dist")
     isolated.install("build[virtualenv]")
     isolated.module("build", "--wheel")
     (wheel,) = dist.iterdir()
@@ -46,16 +48,18 @@
     assert add == "3"
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
 @pytest.mark.broken_on_urct()
-@pytest.mark.skipif(
-    sys.platform.startswith("cygwin"), reason="Cygwin fails here with ld errors"
+@pytest.mark.xfail(
+    sys.platform.startswith("cygwin"),
+    reason="Cygwin fails here with ld errors",
+    strict=False,
 )
 @pytest.mark.usefixtures("package_simple_setuptools_ext")
 def test_pep518_pip(isolated):
     isolated.install("-v", ".")
 
     version = isolated.execute(
         "import cmake_example; print(cmake_example.__version__)",
```

### Comparing `scikit_build_core-0.3.1/tests/test_simple_pure.py` & `scikit_build_core-0.3.2/tests/test_simple_pure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import os
 import shutil
 import subprocess
 import sys
+import sysconfig
 from pathlib import Path
 
 import pytest
 from packaging.version import Version
 
 from scikit_build_core.cmake import CMake, CMaker
 
@@ -17,15 +18,15 @@
 has_make = shutil.which("make") is not None or shutil.which("gmake") is not None
 has_ninja = shutil.which("ninja") is not None
 
 
 def prepare_env_or_skip() -> None:
     if (
         "CMAKE_GENERATOR" not in os.environ
-        and not sys.platform.startswith("win32")
+        and not sysconfig.get_platform().startswith("win")
         and not has_make
     ):
         if has_ninja:
             os.environ["CMAKE_GENERATOR"] = "Ninja"
         else:
             pytest.skip("No build system found")
```

### Comparing `scikit_build_core-0.3.1/tests/test_simplest_c.py` & `scikit_build_core-0.3.2/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_skbuild_settings.py` & `scikit_build_core-0.3.2/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/test_wheelfile_utils.py` & `scikit_build_core-0.3.2/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.3.2/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.3.2/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.3.2/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.3.2/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.3.2/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/.gitignore` & `scikit_build_core-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/LICENSE` & `scikit_build_core-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/README.md` & `scikit_build_core-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.1/PKG-INFO` & `scikit_build_core-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.3.1
+Version: 0.3.2
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Examples, https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

