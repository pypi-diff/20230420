# Comparing `tmp/pyrealm-0.8.1.tar.gz` & `tmp/pyrealm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrealm-0.8.1.tar", max compression
+gzip compressed data, was "pyrealm-0.9.0.tar", max compression
```

## Comparing `pyrealm-0.8.1.tar` & `pyrealm-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,57 @@
--rw-r--r--   0        0        0     7388 2022-08-03 14:12:54.548607 pyrealm-0.8.1/README.md
--rw-r--r--   0        0        0     1047 2022-08-03 14:12:54.549192 pyrealm-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1355 2022-08-02 15:28:52.062142 pyrealm-0.8.1/pyrealm/__init__.py
--rw-r--r--   0        0        0     8439 2022-08-03 14:12:54.549704 pyrealm-0.8.1/pyrealm/bounds_checker.py
--rw-r--r--   0        0        0    19825 2022-07-18 08:22:55.188281 pyrealm-0.8.1/pyrealm/param_classes.py
--rw-r--r--   0        0        0   103697 2022-08-03 14:12:54.550658 pyrealm-0.8.1/pyrealm/pmodel.py
--rw-r--r--   0        0        0    13007 2022-06-15 14:54:02.112615 pyrealm-0.8.1/pyrealm/tmodel.py
--rw-r--r--   0        0        0    24710 2022-08-03 14:12:54.551094 pyrealm-0.8.1/pyrealm/utilities.py
--rw-r--r--   0        0        0      164 2022-08-03 14:12:54.551415 pyrealm-0.8.1/pyrealm/version.py
--rw-r--r--   0        0        0     8419 2022-08-03 14:14:46.568518 pyrealm-0.8.1/setup.py
--rw-r--r--   0        0        0     8414 2022-08-03 14:14:46.569031 pyrealm-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     9182 2023-04-20 10:53:49.634585 pyrealm-0.9.0/README.md
+-rw-r--r--   0        0        0     1570 2023-04-20 10:54:05.614935 pyrealm-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-23 10:26:52.085187 pyrealm-0.9.0/pyrealm/.DS_Store
+-rw-r--r--   0        0        0     1045 2023-04-20 10:53:49.645158 pyrealm-0.9.0/pyrealm/__init__.py
+-rw-r--r--   0        0        0      825 2023-04-20 10:53:49.645516 pyrealm-0.9.0/pyrealm/constants/__init__.py
+-rw-r--r--   0        0        0     1041 2023-02-16 11:21:25.767529 pyrealm-0.9.0/pyrealm/constants/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1039 2023-04-20 10:53:51.430653 pyrealm-0.9.0/pyrealm/constants/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4400 2023-04-19 20:21:57.502720 pyrealm-0.9.0/pyrealm/constants/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     4400 2023-04-20 10:53:51.431710 pyrealm-0.9.0/pyrealm/constants/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1004 2023-02-23 11:59:30.409843 pyrealm-0.9.0/pyrealm/constants/__pycache__/competition_const.cpython-310.pyc
+-rw-r--r--   0        0        0      980 2023-04-20 10:53:51.436009 pyrealm-0.9.0/pyrealm/constants/__pycache__/competition_const.cpython-39.pyc
+-rw-r--r--   0        0        0     2226 2023-02-16 11:21:25.771601 pyrealm-0.9.0/pyrealm/constants/__pycache__/hygro_const.cpython-310.pyc
+-rw-r--r--   0        0        0     2202 2023-04-20 10:53:51.437404 pyrealm-0.9.0/pyrealm/constants/__pycache__/hygro_const.cpython-39.pyc
+-rw-r--r--   0        0        0     1821 2023-02-23 11:59:30.411727 pyrealm-0.9.0/pyrealm/constants/__pycache__/isotope_const.cpython-310.pyc
+-rw-r--r--   0        0        0     1777 2023-04-20 10:53:51.438580 pyrealm-0.9.0/pyrealm/constants/__pycache__/isotope_const.cpython-39.pyc
+-rw-r--r--   0        0        0     8432 2023-02-23 11:59:30.413821 pyrealm-0.9.0/pyrealm/constants/__pycache__/pmodel_const.cpython-310.pyc
+-rw-r--r--   0        0        0     8248 2023-04-20 10:53:51.440568 pyrealm-0.9.0/pyrealm/constants/__pycache__/pmodel_const.cpython-39.pyc
+-rw-r--r--   0        0        0     1539 2023-02-23 11:59:30.416944 pyrealm-0.9.0/pyrealm/constants/__pycache__/tmodel_const.cpython-310.pyc
+-rw-r--r--   0        0        0     1483 2023-04-20 10:53:51.443661 pyrealm-0.9.0/pyrealm/constants/__pycache__/tmodel_const.cpython-39.pyc
+-rw-r--r--   0        0        0     3821 2023-04-20 10:53:49.645769 pyrealm-0.9.0/pyrealm/constants/base.py
+-rw-r--r--   0        0        0     1101 2023-04-20 10:53:49.646112 pyrealm-0.9.0/pyrealm/constants/competition_const.py
+-rw-r--r--   0        0        0     2243 2023-04-20 10:53:49.646351 pyrealm-0.9.0/pyrealm/constants/hygro_const.py
+-rw-r--r--   0        0        0     2254 2023-04-20 10:53:49.646556 pyrealm-0.9.0/pyrealm/constants/isotope_const.py
+-rw-r--r--   0        0        0    11994 2023-04-20 10:53:49.646824 pyrealm-0.9.0/pyrealm/constants/pmodel_const.py
+-rw-r--r--   0        0        0     2615 2023-04-20 10:53:49.646950 pyrealm-0.9.0/pyrealm/constants/tmodel_const.py
+-rw-r--r--   0        0        0     5792 2023-04-20 10:53:49.647914 pyrealm-0.9.0/pyrealm/hygro.py
+-rw-r--r--   0        0        0     1924 2023-04-20 10:53:49.648164 pyrealm-0.9.0/pyrealm/pmodel/__init__.py
+-rw-r--r--   0        0        0     2008 2023-04-19 20:21:57.407299 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2006 2023-04-20 10:53:51.421052 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    10058 2023-02-23 11:59:30.399653 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/competition.cpython-310.pyc
+-rw-r--r--   0        0        0     9992 2023-04-20 10:53:51.422120 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/competition.cpython-39.pyc
+-rw-r--r--   0        0        0    14214 2023-04-19 20:21:57.517696 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/fast_slow_scaler.cpython-310.pyc
+-rw-r--r--   0        0        0    14175 2023-04-20 10:53:51.454938 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/fast_slow_scaler.cpython-39.pyc
+-rw-r--r--   0        0        0    22870 2023-02-23 11:59:30.424584 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0        0        0    22854 2023-04-20 10:53:51.709207 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/functions.cpython-39.pyc
+-rw-r--r--   0        0        0     7139 2023-02-23 11:59:30.425573 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/isotopes.cpython-310.pyc
+-rw-r--r--   0        0        0     7102 2023-04-20 10:53:51.710689 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/isotopes.cpython-39.pyc
+-rw-r--r--   0        0        0    39088 2023-03-16 09:56:17.028347 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/pmodel.cpython-310.pyc
+-rw-r--r--   0        0        0    39006 2023-04-20 10:53:51.714628 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/pmodel.cpython-39.pyc
+-rw-r--r--   0        0        0    11929 2023-04-19 20:21:57.763908 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/subdaily.cpython-310.pyc
+-rw-r--r--   0        0        0    11777 2023-04-20 10:53:51.716649 pyrealm-0.9.0/pyrealm/pmodel/__pycache__/subdaily.cpython-39.pyc
+-rw-r--r--   0        0        0    12661 2023-04-20 10:53:49.648398 pyrealm-0.9.0/pyrealm/pmodel/competition.py
+-rw-r--r--   0        0        0    19722 2023-04-20 10:53:49.648788 pyrealm-0.9.0/pyrealm/pmodel/fast_slow_scaler.py
+-rw-r--r--   0        0        0    25422 2023-04-20 10:53:49.649160 pyrealm-0.9.0/pyrealm/pmodel/functions.py
+-rw-r--r--   0        0        0     9120 2023-04-20 10:53:49.649309 pyrealm-0.9.0/pyrealm/pmodel/isotopes.py
+-rw-r--r--   0        0        0    55792 2023-04-20 10:53:49.649846 pyrealm-0.9.0/pyrealm/pmodel/pmodel.py
+-rw-r--r--   0        0        0    20610 2023-04-20 10:53:49.650243 pyrealm-0.9.0/pyrealm/pmodel/subdaily.py
+-rw-r--r--   0        0        0    14141 2023-04-20 10:53:49.650578 pyrealm-0.9.0/pyrealm/tmodel.py
+-rw-r--r--   0        0        0    11631 2023-04-20 10:53:49.650965 pyrealm-0.9.0/pyrealm/utilities.py
+-rw-r--r--   0        0        0     6148 2021-06-17 14:23:36.976085 pyrealm-0.9.0/pyrealm_build_data/.DS_Store
+-rw-r--r--   0        0        0  8340762 2023-04-20 10:54:05.724727 pyrealm-0.9.0/pyrealm_build_data/UK_WFDE5_FAPAR_2018_JuneJuly.nc
+-rw-r--r--   0        0        0      219 2023-04-20 10:54:05.628297 pyrealm-0.9.0/pyrealm_build_data/__init__.py
+-rw-r--r--   0        0        0     2639 2023-04-03 09:29:51.714526 pyrealm-0.9.0/pyrealm_build_data/create_2D_uk_inputs.py
+-rw-r--r--   0        0        0 12489826 2023-04-20 10:54:05.690301 pyrealm-0.9.0/pyrealm_build_data/pmodel_inputs.nc
+-rw-r--r--   0        0        0  1049127 2023-04-20 10:54:05.665276 pyrealm-0.9.0/pyrealm_build_data/subdaily_BE_Vie_2014.csv
+-rw-r--r--   0        0        0    10263 1970-01-01 00:00:00.000000 pyrealm-0.9.0/setup.py
+-rw-r--r--   0        0        0    10109 1970-01-01 00:00:00.000000 pyrealm-0.9.0/PKG-INFO
```

### Comparing `pyrealm-0.8.1/README.md` & `pyrealm-0.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,235 +7,253 @@
 ## Overview
 
 This a Python 3 package intended to provide a common framework for a number of
 related models of plant productivity, growth and demography.
 
 ## Code development
 
+### Package managment
+
+The package uses `poetry` to manage dependencies, generate virtual environments for code
+development and then for package building and publication. You will need to install
+`poetry` to develop the code.
+
+### Source code management
+
 The codebase is developed in `git` with a repository at:
 
-[https://github.com/davidorme/pyrealm](https://github.com/davidorme/pyrealm)
+[](https://github.com/davidorme/pyrealm)
 
 It uses the `git flow` model for development and release. Briefly:
 
-* All code development should happen on the general `develop` branch or on specific
-  `feature/feature_name` branches.
+* All code development should happen specific `feature/feature_name` branches.
+* Pull requests (PR) should be made to merge feature branches into the `develop` branch.
 * Candidate release versions should be made on specific `release/x.y.z` branches
   and these are then committed to the `master` branch only after final checking.
 * The `master` branch should only ever contain commits representing new release
   versions - do not work on the `master` branch.
 
-## Continuous integration
+Both the `develop` and `master` branches are protected on GitHub to avoid accidents!
+
+### Code quality
+
+The project uses the `pre-commit` tool to enforce code quality. The configuration file
+`.pre-commit-config.yaml` shows the details of the tool chain, but `isort`, `black`,
+`flake8` and `markdownlint` are used to maintain code quality. You will need to install
+`pre-commit` to develop package code, and each PR must pass the same set of checks.
+
+### Code testing
+
+#### Using `doctest`
+
+The package docstrings contain `doctest` examples of code use. These are intended to
+demonstrate use and to validate a reference set of inputs against expected outputs. They
+do not provide extensive unit testing! To run the docstring tests, use:
+
+```bash
+python -m doctest pyrealm/pmodel.py
+python -m doctest pyrealm/*.py
+```
+
+For `doctest` on warnings, see the example for `pyrealm.utilities.convert_rh_to_vpd`
+which redirects the stderr to stdout to allow for the warning text to be included in the
+doctest.
+
+#### Using `pytest`
 
-The project uses continuous integration on the Travis platform to check that the
-package is building correctly as changes are committed to Github. The status of
+The `test` directory contains `pytest` modules to provide greater testing of different
+input combinations and to check errors are raised correctly. These are the main tests
+that the package is behaving as expected.
+
+```bash
+pytest
+```
+
+### Continuous integration
+
+The project uses continuous integration via GitHub Actions to check that the package is
+building correctly and that both `doctest` and `pytest` tests are passing. The status of
 builds can be seen at:
 
-[https://travis-ci.com/github/davidorme/pyrealm](https://travis-ci.com/github/davidorme/pyrealm)
+[](https://github.com/davidorme/pyrealm/actions)
 
 ## Documentation
 
 The `pyrealm` package is documented using `sphinx`, with source material in the
-`source` directory.
+`docs/source` directory.
 
-The documentation in `source` uses [Myst Markdown](https://myst-parser.readthedocs.io/en/latest/)
-rather than the standard `sphinx` reStructuredText (`.rst`) format. This is
-because the documentation uses the `myst_nb` extension to `sphinx` that supports
-running documentation as a Jupyter notebook: the built documentation includes
-examples of running code and output plots to demonstrate the use and behaviour
-of the package.
-
-The `sphinx` configuration includes the `sphinx.ext.mathjax`
-extension to support mathematical notation. This has been configured to also
-load the `mhchem` extension, supporting the rendering of chemical notation.
+The documentation in `source` uses [Myst
+Markdown](https://myst-parser.readthedocs.io/en/latest/) rather than the standard
+`sphinx` reStructuredText (`.rst`) format. This is because the documentation uses the
+`myst_nb` extension to `sphinx` that supports running documentation as a Jupyter
+notebook: the built documentation includes examples of running code and output plots to
+demonstrate the use and behaviour of the package.
+
+The `sphinx` configuration includes the `sphinx.ext.mathjax` extension to support
+mathematical notation. This has been configured to also load the `mhchem` extension,
+supporting the rendering of chemical notation.
 
 ### Docstrings
 
-The module codes uses docstrings written in the
-[Google style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+The module codes uses docstrings written in the [Google
+style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 Unlike the main documentation pages, the docstrings in code are written using
 reStructuredText because the `autodoc` functions in `sphinx` currently rely on `rst`
-inputs. This allows the function documentation to be stored alongside the code
-and included simply into the documentation.
+inputs. This allows the function documentation to be stored alongside the code and
+included simply into the documentation.
 
 ### Building the documentation
 
-Additional python packages given in `source/requirements.txt` are needed
-to build the documentation. To actually build the documentation, use
-`make` in the package root, which will use the `Makefile` created by
-`sphinx-quickstart`.
+Additional python packages given in `docs/source/requirements.txt` are needed to build
+the documentation. To actually build the documentation, use `make` in the package root,
+which will use the `Makefile` created by `sphinx-quickstart`.
 
 ```bash
+cd docs
 make html
 ```
 
 ### Online documentation
 
-TODO - change this to github deployment?
-
 The documentation for the package is hosted at:
 
 [](https://pyrealm.readthedocs.io/en/develop/pmodel.html)
 
 This has been configured to build commits to the `master` branch, which should
 generate version specific sets of documentation.
 
 ### Referencing
 
 The documentation uses the `sphinxcontrib-bibtex` package to support citations.
 This uses Latex like citation keys in the documentation to insert references and
 build a bibliography. The reference library in `source/refs.bib` needs to be
-kept up to date with the literature for the project.
-
-At present, that package uses a rather ugly citation style. I'm hoping the
-`sphinx_astrorefs` package will help out, but there is currently an issue
-getting that package to load.
+kept up to date with the literature for the project. The `sphinx_astrorefs` package is
+used to provide an Author Date style citation format.
 
-## Testing
+## Release process
 
-### Developer installation
+Releasing a new version of the package follows the flow below:
 
-Use the local directory as an editable installation of the package
+1. Create a `release` branch from `develop` containing the new release code.
+2. Check that this branch builds correctly, that the documentation builds correctly and
+   that the package publishes to the `test-pypi` repository.
+3. When all is well, create pull requests on GitHub to merge the `release` branch into
+   both `develop` and `master`, along with a version tag for the release.
+4. Once you have updated your local repository, then the tag can be used to build and
+   publish the final version to the main PyPi site.
 
-```sh
-pip install -e .
-```
-
-### Using `doctest`
-
-The package docstrings contain `doctest` examples of code use. These are
-intended to demonstrate use and to validate a reference set of inputs against
-expected outputs. They do not provide extensive unit testing! To run the
-docstring tests, use:
+It is easier if `git` is configured to push new tags along with commits. This
+essentially just means that new releases can be sent with a single commit. This only
+needs to be set once.
 
 ```bash
-python -m doctest pyrealm/pmodel.py
-python -m doctest pyrealm/*.py
+set git config --global push.followTags true
 ```
 
-For `doctest` on warnings, see the example for `pyrealm.utilities.convert_rh_to_vpd`
-which redirects the stderr to stdout to allow for the warning text to be
-included in the doctest.
-
-### Using `pytest`
+### Create the release branch
 
-The `test` directory contains `pytest` modules to provide greater testing of
-different input combinations (scalars and arrays) and to check errors are
-raised correctly.
+Using `git flow` commands as an example to create a new release:
 
-```bash
-pytest
+```sh
+git flow release start new_release
 ```
 
-### Reference values for testing
-
-The sources of the reference inputs and outputs are:
+Obviously, use something specific, not `new_release`! Ideally, you would do a dry run of
+the next step and use the version - but it should be fairly obvious what this will be!
 
-`pmodel` module:
-    Benjamin Stocker's [`rpmodel`](https://github.com/stineb/rpmodel/tree/master/R)
-    implementation of the P-model in R. The `test` directory contains a YAML
-    file of inputs (`test_inputs.yaml`) and an `R` script (`test_output_rpmodel.R`)
-    that are used to generate a larger YAML file (`test_outputs_rpmodel.R`) that
-    are loaded and validated against {mod}`pyrealm.pmodel` by `test_pmodel.py`.
+The `poetry version` command can then be used to bump the version number. Note that the
+command needs a 'bump rule', which sets which part of the semantic version number to
+increment (`major`, `minor` or `patch`). For example:
 
-## Continuous Integration
+```sh
+poetry version patch
+```
 
-## Git flow
+This updates `pyproject.toml`. At present, the package is set up so that you also *have
+to update the version number in `pyrealm/version.py`* to match manually.
 
-### Configure `git`
+### Publish and test the release branch
 
-It is easier if `git` is configured to push new tags along with commits. This
-essentially just means that new releases can be sent with a single commit,
-which is simpler and saves Travis from building both the the code commit and
-then the tagged version. This only needs to be set once.
+With those changes committed, publish the release branch:
 
-```bash
-set git config --global push.followTags true
+```sh
+git commit -m "Version bump" pyrealm/version.py
+git flow release publish new_release
 ```
 
-Using git-flow and travis
-
-Use git flow to create a release
+The GitHub Actions will then ensure that the code passes quality assurance and then runs
+the test suites on a range of Python versions and operating systems.
 
-```bash
-git flow release start 0.3.0
-```
+### Check package publication
 
-and then bump the version number in `version.py`.
-
-Check the package builds and installs locally:
+The `sdist` and `wheel` builds for the package can then be built locally using `poetry`
 
 ```bash
-python setup.py sdist bdist_wheel
+poetry build
 ```
 
-Commit the version number change and then publish the branch:
+The first time this is run, `poetry` needs to be configured to add the Test PyPi
+repository and an API token from that site. Note that accounts are not shared between
+the Test and main PyPi sites: the API token for `test-pypi` is different from
+`pypi` and you have to log in to each system separately and generate a token on each.
 
 ```sh
-git commit -m "Version bump" pyrealm/version.py
-git flow release publish x.y.z
+poetry config repositories.test-pypi https://test.pypi.org/legacy/
+poetry config pypi-token.test-pypi <your-token>
 ```
 
-to get the branch onto the origin repository and hence into Travis.
-
-### Use twine to check it passes onto testpypi
-
-We are using `twine` to publish versions to PyPi, and using the `testpypi`
-sandbox to check release candidates are accepted. This needs an account
-for both pypi and testpypi.
-
-Remembering to change the version number, use `twine` to upload the built
-versions to the `testpypi` site:
+The built packages can then be published to `test-pypi` using:
 
 ```sh
-twine upload -r testpypi dist/*x.y.z*
+poetry publish -r test-pypi
 ```
 
 ### Check the documentation builds
 
 Log in to:
 
 [](https://readthedocs.org)
 
-which is the admin site controlling the build process. From the Versions
-tab, activate the `release/x.y.z` branch and wait for it to build. Check
-the Builds tab to see that it has built successfully and maybe check
-updates! If it has built succesfully, then go back to the Versions tab
-and deactivate and hide the branch.
-
-## Success
-
-Once all seems well,  the next step is to finish the release, which merges
-changes into `develop` and into a tagged commit on `master`. You then need
-to checkout the master branch and push the new version and tag to GitHub.
+which is the admin site controlling the build process. From the Versions tab, activate
+the `release/new_release` branch and wait for it to build. Check the Builds tab to see
+that it has built successfully and maybe check updates! If it has built succesfully, do
+check pages to make sure that page code has executed successfully, and then go back to
+the Versions tab and deactivate and hide the branch.
 
-```bash
-git flow release finish x.y.z
-git checkout master
-git push
-```
+### Create pull requests into `master` and `develop`
 
-## PyPi upload
+If all is well, then two PRs need to be made on GitHub:
 
-To upload the new version to the main PyPi site, run the build process again
-in the `master` branch to get the release builds:
+* The `release` branch into `master`, to bring all commits since the last release and
+  any fixes on release into `master`.
+* The `release` branch into `develop`, to bring any `release` fixes back into `develop`.
 
-```sh
-python setup.py sdist bdist_wheel
-```
+Once both of those have been merged, the `feature` branch can be deleted.
 
-And then release the distribution using `twine` for use via `pip` - this time
-not using the `testpypi` sandbox.
+### Tag, build and publish
+
+Once the `origin` repository is merged, then use `git pull` to bring `develop` and
+`master` up to date on a local repo. Then, create a tag using the release version.
 
 ```sh
-twine upload dist/*x.y.z*
+git checkout master
+git tag <version>
+git push --tags
 ```
 
-Now:
+The final commit on `master` is now tagged with the release version. You can add tags on
+the GitHub website, but only by using the GitHub release system and we are using PyPi to
+distribute package releases.
 
-* **switch back to `develop`!**
+Before publishing a package to the main PyPi site for the first time, you need to set an
+API token for PyPi.
 
 ```sh
-git checkout develop
+poetry config pypi-token.pypi <your-token>
 ```
 
-* Bump the version number to add `.post9000` to show the code is in development again.
+And now you can build the packages from `master` and publish.
+
+```sh
+poetry build
+poetry publish
+```
```

### Comparing `pyrealm-0.8.1/pyrealm/__init__.py` & `pyrealm-0.9.0/pyrealm/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,41 @@
 """The pyrealm package.
 
 TODO: complete this documentation
 """
 
+import importlib.metadata
 import os
 import warnings
+from typing import Optional, Type, Union
 
-# _ROOT = os.path.abspath(os.path.dirname(__file__))
-#
-#
-# def get_data_path(path):
-#     return os.path.join(_ROOT, 'data', path)
+__version__ = importlib.metadata.version("pyrealm")
 
 
 class ExperimentalFeatureWarning(Warning):
     """Warn about experimental features.
 
     This is just a simple wrapper on the base Warning to issue clearer warnings about
     experimental features in the code.
     """
 
-    def __init__(self, message) -> None:
+    def __init__(self, message: str) -> None:
         self.message = message
 
     def __str__(self) -> str:
         return repr(self.message)
 
 
 # Setup warnings to simpler one line warning
 def warning_on_one_line(
-    message: str, category: str, filename: str, lineno: int, file=None, line=None
-):
+    message: Union[Warning, str],
+    category: Type[Warning],
+    filename: str,
+    lineno: int,
+    line: Optional[str] = None,
+) -> str:
     """Provide a simple one line warning for use in docstrings."""
     filename = os.path.join("pyrealm", os.path.basename(filename))
     return "%s:%s: %s: %s\n" % (filename, lineno, category.__name__, message)
 
 
 warnings.formatwarning = warning_on_one_line
-
-# # And provide a decorator to catch warnings in doctests
-# # https://stackoverflow.com/questions/2418570/
-
-# def stderr_to_stdout(func):
-#     def wrapper(*args):
-#         stderr_bak = sys.stderr
-#         sys.stderr = sys.stdout
-#         try:
-#             return func(*args)
-#         finally:
-#             sys.stderr = stderr_bak
-#     return wrapper
```

### Comparing `pyrealm-0.8.1/pyrealm/bounds_checker.py` & `pyrealm-0.9.0/pyrealm/utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,288 @@
-"""The bounds_checker module.
+"""The :mod:`~pyrealm.utilities` module provides shared utility functions used to:
 
-This module contains utility functions to handle bounds checking on the inputs to
-functions and methods in the `pyrealm` package. Some functions are only
-well-behaved with given bounds and bounds checking also provides a (partial)
-check on the units being provided.
-"""
+* check input arrays to functions have congruent shapes
+* summarize object attributes in a tabular format
+* apply bounds checking to inputs to functions and methods in the ``pyrealm`` package.
+
+Some functions in ``pyrealm`` are only well-behaved with given bounds and bounds
+checking also provides a (partial) check on the units being provided.
+
+An earlier implementation of bounds checking used a subclass of
+:class:`numpy.ma.MaskedArray` . The intention was that a checked array becomes a thing
+that carries with it a description of any applied constraint, which sounds appealing
+but...
+
+1) MaskedArrays have a performance hit.
+2) Subclasses are 'contagious': so x * subclass returns an object of class subclass.
+   That then requires the subclass to be extended to handle all required methods.
+3) NaN handling. Numpy has np.nan - and masked arrays do handle _masked_ np.nan values,
+   but not unmasked ones:
+
+.. :code-block: python
+
+  >>> import numpy as np
+  >>> x = np.ma.masked_array([1,2,np.nan, 4], mask=[1,0,0,1])
+  >>> x.mean()
+  nan
+  >>> x = np.ma.masked_array([1,2,np.nan, 4], mask=[1,0,1,0])
+  >>> x.mean()
+  3.0
+
+So the general approach here is now:
+
+* a bounds checker function that tests if data exceeds bounds and warns when it does.
+* a bounds mask function that returns np.ndarrays masked using np.nan when values are
+  out of the applied bounds. Because np.nan is a _float_ value, masking is always
+  applied to a float version of the input.
+
+Note that this means that the codebase then needs to systematically use nan-aware
+functions and possibly using bottleneck for speed. Part of the problem here is that
+Numpy lacks a general solution to missing data:
+https://numpy.org/neps/nep-0026-missing-data-summary
+"""  # noqa: D205, D415
 
-from numbers import Number
 from typing import Union
 
 import numpy as np
+import tabulate
+from numpy.typing import NDArray
 
 from pyrealm import warnings
 
-# DESIGN NOTES: DO 18/08/21
-#
-# As originally implemented (still commented below), this module provided a
-# subclass of numpy.ma.core.MaskedArray. The intention was that a constrained
-# array becomes a thing that carries with it a description of its constraints,
-# which sounds appealing but...
-#
-# 1) MaskedArrays have a performance hit.
-# 2) Subclasses are 'contagious': so x * subclass returns an object of class
-#    subclass. The attributes of that subclass weren't being set and I suspect
-#    that is fixable but it doesn't make sense to do so (unless you were mad
-#    enough to implement bounds on _all_ values)
-# 3) NaN handling. Numpy has np.nan - and masked arrays do handle _masked_
-#    np.nan values, but not unmasked ones:
-#
-#   x = np.ma.masked_array([1,2,np.nan, 4], mask=[1,0,0,1])
-#   x.mean()
-#   Out[49]: nan
-#   x = np.ma.masked_array([1,2,np.nan, 4], mask=[1,0,1,0])
-#   x.mean()
-#   Out[51]: 3.0
-#
-# So the general approach here is now:
-#
-# - a data constraint function that returns simple np.ndarrays or np.nan
-# - uses np.nan for both missing / out of range
-# - (maybe) has a public mechanism for setting those constraints, rather than
-#   hard coding them. But if the ranges are well documented and sane, then
-#   this might be fussy, so parking for now.
-#
-# This is simpler and cleaner but the codebase then needs to systematically
-# use nan-aware functions and possibly using bottleneck for speed. Part of
-# the problem here is that Numpy lacks a general solution to missing  data:
-#   - https://numpy.org/neps/nep-0026-missing-data-summary
-#
-# Two issues:
-# 1) np.nan is a _float_ value and so this can only be applied to float types
-#    and hence some type conversion happens.
-# 2) The ability to check for already checked data is lost from the previous
-#    implementation. This requires the array object to carry attributes, and
-#    that implies subclasses.
-#
-# NOTES: DO 20/11/2021
-#
-# Actually imposing constraints and enforcing masking is too heavy handed
-# and causes user issues. So, instead retain some of this as a mechanism for
-# helping users sanitise inputs, but provide a simple routine to check whether
-# values are sane.
+
+def check_input_shapes(*args: Union[float, int, np.generic, np.ndarray, None]) -> tuple:
+    """Check sets of input variables have congruent shapes.
+
+    This helper function validates inputs to check that they are either scalars or
+    arrays and then that any arrays of the same shape. It returns a tuple of the common
+    shape of the arguments, which is (1,) if all the arguments are scalar.
+
+    Parameters:
+        *args: A set of numpy arrays or scalar values
+
+    Returns:
+        The common shape of any array inputs or 1 if all inputs are scalar.
+
+    Raises:
+        ValueError: if the inputs contain arrays of differing shapes.
+
+    Examples:
+        >>> check_input_shapes(np.array([1,2,3]), 5)
+        (3,)
+        >>> check_input_shapes(4, 5)
+        1
+        >>> check_input_shapes(np.array([1,2,3]), np.array([1,2]))
+        Traceback (most recent call last):
+        ...
+        ValueError: Inputs contain arrays of different shapes.
+    """
+
+    # Collect the shapes of the inputs
+    shapes = set()
+
+    # DESIGN NOTES - currently allow:
+    #   - scalars,
+    #   - 0 dim ndarrays (also scalars but packaged differently)
+    #   - 1 dim ndarrays with only a single value
+
+    for val in args:
+        if isinstance(val, np.ndarray):
+            # Note that 0-dim ndarrays (which are scalars) pass through as do
+            # one dimensional arrays with a single value (also a scalar)
+            if not (val.ndim == 0 or val.shape == (1,)):
+                shapes.add(val.shape)
+        # elif isinstance(val, Series):
+        #    # Note that 0-dim ndarrays (which are scalars) pass through
+        #    if val.ndim > 0:
+        #        shapes.add(val.shape)
+        elif val is None or isinstance(val, (float, int, np.generic)):
+            pass  # No need to track scalars and optional values pass None
+        else:
+            raise ValueError(f"Unexpected input to check_input_shapes: {type(val)}")
+
+    # shapes can be an empty set (all scalars) or contain one common shape
+    # otherwise raise an error
+    if len(shapes) > 1:
+        raise ValueError("Inputs contain arrays of different shapes.")
+
+    if len(shapes) == 1:
+        return shapes.pop()
+
+    return (1,)
+
+
+def summarize_attrs(
+    obj: object, attrs: list, dp: int = 2, repr_head: bool = True
+) -> None:
+    """Print a summary table of object attributes.
+
+    This helper function prints a simple table of the mean, min, max and nan
+    count for named attributes from an object for use in class summary
+    functions.
+
+    Args:
+        obj: An object with attributes to summarize
+        attrs: A list of strings of attribute names, or a list of 2-tuples
+            giving attribute names and units.
+        dp: The number of decimal places used in rounding summary stats.
+        repr_head: A boolean indicating whether to show the object
+            representation before the summary table.
+    """
+
+    # Check inputs
+    if not isinstance(attrs, list):
+        raise RuntimeError("attrs input not a list")
+
+    # Create a list to hold variables and summary stats
+    ret = []
+
+    if len(attrs):
+        first = attrs[0]
+
+        # TODO: - not much checking for consistency here!
+        if isinstance(first, str):
+            has_units = False
+            attrs = [(vl, None) for vl in attrs]
+        else:
+            has_units = True
+
+        # Process the attributes
+        for attr_entry in attrs:
+            attr = attr_entry[0]
+            unit = attr_entry[1]
+
+            data = getattr(obj, attr)
+
+            # Avoid masked arrays - run into problems with edge cases with all NaN
+            if isinstance(data, np.ma.core.MaskedArray):
+                # Mypy complains about filled being untyped?
+                data = data.filled(np.nan)  # type: ignore
+
+            # Add the variable and stats to the list to be displayed
+            attr_row = [
+                attr,
+                np.round(np.nanmean(data), dp),
+                np.round(np.nanmin(data), dp),
+                np.round(np.nanmax(data), dp),
+                np.count_nonzero(np.isnan(data)),
+            ]
+            if has_units:
+                attr_row.append(unit)
+
+            ret.append(attr_row)
+
+    if has_units:
+        hdrs = ["Attr", "Mean", "Min", "Max", "NaN", "Units"]
+    else:
+        hdrs = ["Attr", "Mean", "Min", "Max", "NaN"]
+
+    if repr_head:
+        print(obj)
+
+    print(tabulate.tabulate(ret, headers=hdrs))
+
+
+def _get_interval_functions(interval_type: str = "[]") -> tuple[np.ufunc, np.ufunc]:
+    """Converts interval notation type to appropriate functions.
+
+    The interval type should be one of ``[]``, ``()``, ``[)`` or ``(]``. The function
+    returns a two tuple of ``numpy.ufunc`` functions that implement the appropriate
+    lower and upper boundaries given the interval type.
+
+    Args:
+        interval_type: A string describing the interval bounds
+    """
+
+    # Implement the interval type
+    if interval_type not in ["[]", "()", "[)", "(]"]:
+        raise ValueError(f"Unknown interval type: {interval_type}")
+
+    # Default open interval traps values less or greater than
+    lower_func: np.ufunc = np.less
+    upper_func: np.ufunc = np.greater
+
+    # Closed intervals replace functions with less_eq/greater_wq
+    if interval_type[0] == "(":
+        lower_func = np.less_equal
+
+    if interval_type[1] == ")":
+        upper_func = np.greater_equal
+
+    return lower_func, upper_func
 
 
 def bounds_checker(
-    values: Union[np.ndarray, Number],
-    lower: Number = -np.infty,
-    upper: Number = np.infty,
+    values: NDArray,
+    lower: float = -np.infty,
+    upper: float = np.infty,
     interval_type: str = "[]",
     label: str = "",
     unit: str = "",
-):
+) -> NDArray:
     r"""Check inputs fall within bounds.
 
     This is a simple pass through function that tests whether the values fall within
     the bounds specified and issues a warning when this is not the case
 
     Args:
-        values: An np.ndarray object or number
+        values: An np.ndarray
         lower: The value of the lower constraint
         upper: The value of the upper constraint
         interval_type: The interval type of the constraint ('[]', '()', '[)', '(]')
         label: A string giving a descriptive label of the variable for use in warnings.
         unit: A string specifying the expected units.
 
     Returns:
         The function returns the contents of values.
 
     Examples:
         >>> vals = np.array([-15, 20, 30, 124], dtype=np.float)
         >>> vals_c = bounds_checker(vals, 0, 100, label='temperature', unit='°C')
     """
 
-    # Implement the interval type
-    if interval_type not in ["[]", "()", "[)", "(]"]:
-        raise RuntimeWarning(f"Unknown interval type: {interval_type}")
-
-    if interval_type[0] == "[":
-        lower_func = np.less
-    else:
-        lower_func = np.less_equal
-
-    if interval_type[1] == "]":
-        upper_func = np.greater
-    else:
-        upper_func = np.greater_equal
+    # Get the interval functions
+    lower_func, upper_func = _get_interval_functions(interval_type)
 
-    # Do the input values contain out of bound values? These tests are not
-    # sensitive to dtype, float or int inputs and return either numpy.bool_
-    # or np.ndarray with dtype 'bool', both of which support the sum() method
+    # Do the input values contain out of bound values?
     out_of_bounds = np.logical_or(lower_func(values, lower), upper_func(values, upper))
 
     if out_of_bounds.sum():
         warnings.warn(
             f"Variable {label} ({unit}) contains values outside "
             f"the expected range ({lower},{upper}). Check units?"
         )
 
     return values
 
 
-def input_mask(
-    inputs: Union[np.ndarray, Number],
-    lower: Number = -np.infty,
-    upper: Number = np.infty,
+def bounds_mask(
+    inputs: NDArray,
+    lower: float = -np.infty,
+    upper: float = np.infty,
     interval_type: str = "[]",
     label: str = "",
-):
+) -> NDArray[np.floating]:
     r"""Mask inputs that do not fall within bounds.
 
-    This function constrains the values in inputs, replacing values outside
-    the provided interval with np.nan. Because np.nan is a float, when any data
-    is out of bounds, the returned values are always float arrays or np.nan.
+    This function constrains the values in inputs, replacing values outside the provided
+    interval with np.nan. Because np.nan is only defined for float types, the function
+    will always return a float array.
 
     Args:
-        inputs: An np.ndarray object or number
+        inputs: An np.ndarray
         lower: The value of the lower constraint
         upper: The value of the upper constraint
         interval_type: The interval type of the constraint ('[]', '()', '[)', '(]')
         label: A string giving a descriptive label of the constrained contents
             used in reporting.
 
     Returns:
         If no data is out of bounds, the original inputs are returned, otherwise
-        a float np.ndarray object with out of bounds values replaced with np.nan
-        or np.nan for number or zero dimension ndarrays.
+        a float np.ndarray object with out of bounds values replaced with np.nan.
 
     Examples:
         >>> vals = np.array([-15, 20, 30, 124], dtype=np.float)
         >>> np.nansum(vals)
         159.0
         >>> vals_c = input_mask(vals, 0, 100, label='temperature')
         >>> np.nansum(vals_c)
@@ -157,73 +291,47 @@
         >>> np.nansum(vals_c)
         174.0
         >>> vals_c = input_mask(vals, 0, 124, interval_type='[)', label='temperature')
         >>> np.nansum(vals_c)
         50.0
     """
 
-    # Implement the interval type
-    if interval_type not in ["[]", "()", "[)", "(]"]:
-        raise RuntimeWarning(f"Unknown interval type: {interval_type}")
+    # Get the interval functions
+    lower_func, upper_func = _get_interval_functions(interval_type)
 
-    if interval_type[0] == "[":
-        lower_func = np.less
-    else:
-        lower_func = np.less_equal
-
-    if interval_type[1] == "]":
-        upper_func = np.greater
-    else:
-        upper_func = np.greater_equal
+    # Raise error for non-array input
+    if not isinstance(inputs, np.ndarray):
+        raise TypeError(f"Cannot set bounds on {type(inputs)}")
 
-    # Do the input values contain out of bound values? These tests are not
-    # sensitive to dtype, float or int inputs and return either numpy.bool_
-    # or np.ndarray with dtype 'bool', both of which support the sum() method
+    # Do the input values contain out of bound values?
     mask = np.logical_or(lower_func(inputs, lower), upper_func(inputs, upper))
 
     # Check if any masking needs to be done
-    if mask.sum():
-
-        if isinstance(mask, np.bool_):
-            # If mask is np.bool_ then a scalar or zero dimension ndarray was passed,
-            # so return np.nan, implicitly converting the input to a float.
-
-            warnings.warn(
-                f"Scalar value {inputs} set to NaN "
-                f"using {interval_type[0]}{lower}, {upper}{interval_type[1]} "
-                f"bounds on {label}",
-                category=RuntimeWarning,
-            )
-
-            return np.nan
-
-        if isinstance(mask, np.ndarray):
-            # If an ndarray, then we need a float version to set np.nan and we
-            # copy to avoid modifying the original input
-            if not np.issubdtype(inputs.dtype, np.floating):
-                # Copies implicitly
-                outputs = inputs.astype(np.float)
-            else:
-                outputs = inputs.copy()
-
-            # Count the existing number of NaN values - impossible to have nan
-            # in an integer input but isnan works with any input.
-            initial_na_count = np.isnan(inputs).sum()
-
-            # Fill in np.nan where values around outside constraints
-            outputs[mask] = np.nan
-
-            final_na_count = np.isnan(outputs).sum()
-
-            # Report
-            warnings.warn(
-                f"{final_na_count - initial_na_count} values set to NaN "
-                f"using {interval_type[0]}{lower}, {upper}{interval_type[1]} "
-                f"bounds on {label}",
-                category=RuntimeWarning,
-            )
+    if not mask.sum():
+        return inputs
 
-            return outputs
+    # If an ndarray, then we need a float version to set np.nan and we copy to avoid
+    # modifying the original input. Using type
+    if not np.issubdtype(inputs.dtype, np.floating):
+        # Copies implicitly
+        outputs = inputs.astype(np.float32)
+    else:
+        outputs = inputs.copy()
 
-        raise NotImplementedError(f"Cannot set bounds on {type(inputs)}")
+    # Count the existing number of NaN values - impossible to have nan in an integer
+    # input but isnan works with any input.
+    initial_na_count = np.isnan(inputs).sum()
+
+    # Fill in np.nan where values around outside constraints
+    outputs[mask] = np.nan
+
+    final_na_count = np.isnan(outputs).sum()
+
+    # Report
+    warnings.warn(
+        f"{final_na_count - initial_na_count} values set to NaN "
+        f"using {interval_type[0]}{lower}, {upper}{interval_type[1]} "
+        f"bounds on {label}",
+        category=RuntimeWarning,
+    )
 
-    return inputs
+    return outputs
```

### Comparing `pyrealm-0.8.1/pyrealm/tmodel.py` & `pyrealm-0.9.0/pyrealm/tmodel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-"""The tmodel Module.
-
-This module provides an implementation of the T Model of plant growth given
-an estimate of gross primary productivity (GPP).
+"""The :mod:`~pyrealm.tmodel` module provides an implementation of the T Model of plant
+growth given an estimate of gross primary productivity (GPP).
 
 * The growth form and productivity allocation model of a plant is set using
-    :class:`~pyrealm.param_classes.TModelTraits`.
+    :class:`~pyrealm.constants.tmodel_const.TModelTraits`.
 * The class :class:`~pyrealm.tmodel.TTree` is used to generate an instance of a
-  plant to be simulated, with methods :meth:`~pyrealm.tmodel.TTree.set_diameter`
+  plant to be simulated, with methods :meth:`~pyrealm.tmodel.TTree.reset_diameters`
   and :meth:`~pyrealm.tmodel.TTree.calculate_growth` to calculate the plant
   geometry for a given diameter or predict growth from estimated GPP.
 * The function :func:`~pyrealm.tmodel.grow_ttree` predicts plant growth through
   time given a time series of GPP.
-"""
-
-from typing import Tuple, Union
+"""  # noqa: D205, D415
 
 import numpy as np
+from numpy.typing import NDArray
 
-from pyrealm.param_classes import TModelTraits
-from pyrealm.utilities import check_input_shapes
+from pyrealm.constants.tmodel_const import TModelTraits
 
 # Design Notes:
 #
 # One functionally easy thing to do the TTree object is to expose the geometry
 # methods (e.g. by having TTree.calculate_crown_area()) to allow users to
 # subclass the object and substitute their own geometry. Which is neat but the
 # geometry and growth are not separate and there is no guarantee that a
@@ -30,368 +26,384 @@
 # natural solution to people wanting to tinker with the geometry but not going
 # there now.
 
 
 class TTree:
     """Model plant growth using the T model.
 
-    This class provides an implementation of the calculations of tree geometry,
-    mass and growth described by :cite:`Li:2014bc`. All of the properties of
-    the T model are derived from a set of traits (see :class:`~pyrealm.tmodel.Traits`),
-    stem diameter measurements and estimates of gross primary productivity.
-
-    See the details of :meth:`~pyrealm.tmodel.TTree.set_diameter` and
-    :meth:`~pyrealm.tmodel.TTree.calculate_growth` for details of the properties
-    and calculations.
+    This class provides an implementation of the calculations of tree geometry, mass and
+    growth described by :cite:t:`Li:2014bc`. All of the properties of the T model are
+    derived from a set of traits (see
+    :class:`~pyrealm.constants.tmodel_const.TModelTraits`), stem diameter measurements
+    and estimates of gross primary productivity.
+
+    See the details of :meth:`~pyrealm.tmodel.TTree.reset_diameters` and
+    :meth:`~pyrealm.tmodel.TTree.calculate_growth` for details of the properties and
+    calculations.
 
     Args:
-        traits: An object of class :class:`~pyrealm.param_classes.TModelTraits`
+        traits: An object of class :class:`~pyrealm.constants.tmodel_const.TModelTraits`
+        diameters: A float or np.array of stem diameters.
     """
 
-    def __init__(self, traits: TModelTraits = TModelTraits()):
-
-        self.traits = traits
+    def __init__(
+        self,
+        diameters: NDArray,
+        traits: TModelTraits = TModelTraits(),
+    ) -> None:
+        self.traits: TModelTraits = traits
 
         # The diameter is used to define all of the geometric scaling
-        # based on the trait parameters. It is set by the set_diameter()
-        # method, which then populates the other geometric variables
-        self._diameter = None
-        self._height = None
-        self._crown_fraction = None
-        self._crown_area = None
-        self._mass_stm = None
-        self._mass_fol = None
-        self._mass_swd = None
+        # based on the trait parameters.
+
+        self._diameter: NDArray
+        self._height: NDArray
+        self._crown_fraction: NDArray
+        self._crown_area: NDArray
+        self._mass_stm: NDArray
+        self._mass_fol: NDArray
+        self._mass_swd: NDArray
+
+        self.reset_diameters(diameters)
 
         # Growth is then applied by providing estimated gpp using the
         # calculate_growth() method, which populates the following:
-        self._gpp_raw = None
-        self._gpp_actual = None
-        self._npp = None
-        self._resp_swd = None
-        self._resp_frt = None
-        self._resp_fol = None
-        self._turnover = None
-        self._d_mass_s = None
-        self._d_mass_fr = None
-        self._delta_d = None
-        self._delta_mass_stm = None
-        self._delta_mass_frt = None
+        self.growth_calculated: bool = False
+        self._gpp_raw: NDArray
+        self._gpp_actual: NDArray
+        self._npp: NDArray
+        self._resp_swd: NDArray
+        self._resp_frt: NDArray
+        self._resp_fol: NDArray
+        self._turnover: NDArray
+        self._d_mass_s: NDArray
+        self._d_mass_fr: NDArray
+        self._delta_d: NDArray
+        self._delta_mass_stm: NDArray
+        self._delta_mass_frt: NDArray
+
+    def _check_growth_calculated(self, property: str) -> NDArray:
+        """Helper function to return growth values if calculated.
+
+        This acts as a gatekeeper to make sure that a growth property is not returned
+        before calculate_growth() has been run on the current diameters.
+
+        Args:
+            property: The property value to return if available.
+        """
+        if not self.growth_calculated:
+            raise RuntimeError("Growth estimates not calculated: use calculate_growth")
+
+        return getattr(self, property)
 
     @property
-    def diameter(self):
-        """Fetch the plant diameter."""
+    def diameter(self) -> NDArray:
+        """Individual diameter (m)."""  # noqa: D402
         return self._diameter
 
     @property
-    def height(self):
-        """Fetch the plant height."""
+    def height(self) -> NDArray:
+        """Individual height (m)."""  # noqa: D402
         return self._height
 
     @property
-    def crown_fraction(self):
-        """Fetch the plant crown fraction."""
+    def crown_fraction(self) -> NDArray:
+        """Individual crown fraction (unitless)."""
         return self._crown_fraction
 
     @property
-    def crown_area(self):
-        """Fetch the plant crown area."""
+    def crown_area(self) -> NDArray:
+        """Individual crown area (m2)."""
         return self._crown_area
 
     @property
-    def mass_swd(self):
-        """Fetch the plant softwood mass."""
+    def mass_swd(self) -> NDArray:
+        """Individual softwood mass (kg)."""
         return self._mass_swd
 
     @property
-    def mass_stm(self):
-        """Fetch the plant stem mass."""
+    def mass_stm(self) -> NDArray:
+        """Individual stem mass (kg)."""
         return self._mass_stm
 
     @property
-    def mass_fol(self):
-        """Fetch the plant foliage mass."""
+    def mass_fol(self) -> NDArray:
+        """Individual foliage mass (kg)."""
         return self._mass_fol
 
     @property
-    def gpp_raw(self):
-        """Fetch the raw gross primary productivity."""
-        return self._gpp_raw
+    def gpp_raw(self) -> NDArray:
+        """Raw gross primary productivity."""
+        return self._check_growth_calculated("_gpp_raw")
 
     @property
-    def gpp_actual(self):
-        """Fetch the actual gross primary productivity."""
-        return self._gpp_actual
+    def gpp_actual(self) -> NDArray:
+        """Actual gross primary productivity."""
+        return self._check_growth_calculated("_gpp_actual")
 
     @property
-    def resp_swd(self):
-        """Fetch the plant softwood respiration."""
-        return self._resp_swd
+    def resp_swd(self) -> NDArray:
+        """Individual softwood respiration costs."""
+        return self._check_growth_calculated("_resp_swd")
 
     @property
-    def resp_frt(self):
-        """Fetch the plant fine root respiration."""
-        return self._resp_frt
+    def resp_frt(self) -> NDArray:
+        """Individual fine root respiration costs."""
+        return self._check_growth_calculated("_resp_frt")
 
     @property
-    def resp_fol(self):
-        """Fetch the plant foliar respiration."""
-        return self._resp_fol
+    def resp_fol(self) -> NDArray:
+        """Individual foliar respiration costs."""
+        return self._check_growth_calculated("_resp_fol")
 
     @property
-    def npp(self):
-        """Fetch the net primary productivity."""
-        return self._npp
+    def npp(self) -> NDArray:
+        """Net primary productivity."""
+        return self._check_growth_calculated("_npp")
 
     @property
-    def turnover(self):
-        """Fetch the plant turnover."""
-        return self._turnover
+    def turnover(self) -> NDArray:
+        """Plant turnover."""
+        return self._check_growth_calculated("_turnover")
 
     @property
-    def d_mass_s(self):
-        """Fetch the plant change in mass."""
-        return self._d_mass_s
+    def d_mass_s(self) -> NDArray:
+        """Individual relative change in mass."""
+        return self._check_growth_calculated("_d_mass_s")
 
     @property
-    def d_mass_fr(self):
-        """Fetch the plant change in fine root mass."""
-        return self._d_mass_fr
+    def d_mass_fr(self) -> NDArray:
+        """Individual relative change in fine root mass."""
+        return self._check_growth_calculated("_d_mass_fr")
 
     @property
-    def delta_d(self):
-        """Fetch the plant change in diameter."""
-        return self._delta_d
+    def delta_d(self) -> NDArray:
+        """Individual change in diameter."""
+        return self._check_growth_calculated("_delta_d")
 
     @property
-    def delta_mass_stm(self):
-        """Fetch the plant change in stem mass."""
-        return self._delta_mass_stm
+    def delta_mass_stm(self) -> NDArray:
+        """Individual total change in stem mass."""
+        return self._check_growth_calculated("_delta_mass_stm")
 
     @property
-    def delta_mass_frt(self):
-        """Fetch the plant change in fine root mass."""
-        return self._delta_mass_frt
+    def delta_mass_frt(self) -> NDArray:
+        """Individual total change in fine root mass."""
+        return self._check_growth_calculated("_delta_mass_frt")
 
-    def set_diameter(self, values: Union[float, np.ndarray]):
-        """Set the stem diameter for the T model.
+    def reset_diameters(self, values: NDArray) -> None:
+        """Reset the stem diameters for the T model.
 
-        The set_diameter method sets the diameter values and then uses these
-        values to populate the geometric and mass properties that scale with
-        stem diameter.
+        The set_diameter method can be used to reset the diameter values and then uses
+        these values to populate the geometric and mass properties that scale with stem
+        diameter.
 
         * Height (m, ``height``, :math:`H`):
 
         .. math::
 
             H = H_{max} ( 1 - e^{a D/ H_{max}}
 
         TODO: complete this description.
         """
 
         self._diameter = values
 
         # Height of tree from diameter, Equation (4) of Li ea.
         self._height = self.traits.h_max * (
-            1 - np.exp(-self.traits.a_hd * self.diameter / self.traits.h_max)
+            1 - np.exp(-self.traits.a_hd * self._diameter / self.traits.h_max)
         )
 
         # Crown area of tree, Equation (8) of Li ea.
         self._crown_area = (
             ((np.pi * self.traits.ca_ratio) / (4 * self.traits.a_hd))
-            * self.diameter
-            * self.height
+            * self._diameter
+            * self._height
         )
 
         # Crown fraction, Equation (11) of Li ea.
-        self._crown_fraction = self.height / (self.traits.a_hd * self.diameter)
+        self._crown_fraction = self._height / (self.traits.a_hd * self._diameter)
 
         # Masses
         self._mass_stm = (
-            (np.pi / 8) * (self.diameter**2) * self.height * self.traits.rho_s
+            (np.pi / 8) * (self._diameter**2) * self._height * self.traits.rho_s
         )
-        self._mass_fol = self.crown_area * self.traits.lai * (1 / self.traits.sla)
+        self._mass_fol = self._crown_area * self.traits.lai * (1 / self.traits.sla)
         self._mass_swd = (
-            self.crown_area
+            self._crown_area
             * self.traits.rho_s
-            * self.height
-            * (1 - self.crown_fraction / 2)
+            * self._height
+            * (1 - self._crown_fraction / 2)
             / self.traits.ca_ratio
         )
 
-        # Clear any calculated growth values
-        self._gpp_raw = None
-        self._gpp_actual = None
-        self._npp = None
-        self._resp_swd = None
-        self._resp_frt = None
-        self._resp_fol = None
-        self._turnover = None
-        self._d_mass_s = None
-        self._d_mass_fr = None
-        self._delta_d = None
-        self._delta_mass_stm = None
-        self._delta_mass_frt = None
+        # Flag any calculated growth values as outdated
+        self.growth_calculated = False
 
-    def calculate_growth(self, gpp):
+    def calculate_growth(self, gpp: NDArray) -> None:
         """Calculate growth predictions given a GPP estimate.
 
-        This method updates the instance with predicted changes in tree
-        geometry, mass and respiration costs from the initial state given an
-        estimate of gross primary productivity (GPP).
+        This method updates the instance with predicted changes in tree geometry, mass
+        and respiration costs from the initial state given an estimate of gross primary
+        productivity (GPP).
 
         Args:
             gpp: Primary productivity
         """
 
         # GPP fixed per m2 of crown
         self._gpp_raw = gpp
-        gpp_unit_cr = self.gpp_raw * (
+        gpp_unit_cr = self._gpp_raw * (
             1 - np.exp(-(self.traits.par_ext * self.traits.lai))
         )
-        self._gpp_actual = self.crown_area * gpp_unit_cr
+        self._gpp_actual = self._crown_area * gpp_unit_cr
 
         # Respiration costs (Eqn 13 of Li ea)
         # - sapwood, fine root and foliage maintenance
-        self._resp_swd = self.mass_swd * self.traits.resp_s
+        self._resp_swd = self._mass_swd * self.traits.resp_s
         self._resp_frt = (
-            self.traits.zeta * self.traits.sla * self.mass_fol * self.traits.resp_r
+            self.traits.zeta * self.traits.sla * self._mass_fol * self.traits.resp_r
         )
-        self._resp_fol = self.gpp_actual * self.traits.resp_f
+        self._resp_fol = self._gpp_actual * self.traits.resp_f
 
         # Net primary productivity
         self._npp = self.traits.yld * (
-            self.gpp_actual - self.resp_fol - self.resp_frt - self._resp_swd
+            self._gpp_actual - self._resp_fol - self._resp_frt - self._resp_swd
         )
 
         # Turnover costs for foliage and fine roots
         self._turnover = (
-            self.crown_area
+            self._crown_area
             * self.traits.lai
             * (
                 (1 / (self.traits.sla * self.traits.tau_f))
                 + (self.traits.zeta / self.traits.tau_r)
             )
         )
 
         # relative increments - these are used to calculate delta_d and
         # then scaled by delta_d to give actual increments
         self._d_mass_s = (
             np.pi
             / 8
             * self.traits.rho_s
-            * self.diameter
+            * self._diameter
             * (
                 self.traits.a_hd
-                * self.diameter
-                * (1 - (self.height / self.traits.h_max))
-                + 2 * self.height
+                * self._diameter
+                * (1 - (self._height / self.traits.h_max))
+                + 2 * self._height
             )
         )
 
         self._d_mass_fr = (
             self.traits.lai
             * ((np.pi * self.traits.ca_ratio) / (4 * self.traits.a_hd))
             * (
-                self.traits.a_hd * self.diameter * (1 - self.height / self.traits.h_max)
-                + self.height
+                self.traits.a_hd
+                * self._diameter
+                * (1 - self._height / self.traits.h_max)
+                + self._height
             )
             * (1 / self.traits.sla + self.traits.zeta)
         )
 
         # Actual increments
-        self._delta_d = (self.npp - self.turnover) / (self.d_mass_s + self.d_mass_fr)
-        self._delta_mass_stm = self.d_mass_s * self.delta_d
-        self._delta_mass_frt = self.d_mass_fr * self.delta_d
+        self._delta_d = (self._npp - self._turnover) / (
+            self._d_mass_s + self._d_mass_fr
+        )
+        self._delta_mass_stm = self._d_mass_s * self._delta_d
+        self._delta_mass_frt = self._d_mass_fr * self._delta_d
+
+        self.growth_calculated = True
 
 
 def grow_ttree(
-    gpp: Union[float, np.ndarray],
-    d_init: Union[float, np.ndarray],
+    gpp: NDArray,
+    d_init: NDArray,
     time_axis: int,
     traits: TModelTraits = TModelTraits(),
-    outvars: Tuple[str, ...] = ("diameter", "height", "crown_area", "delta_d"),
-) -> dict:
-    """Fit a growth time series using the T Model.
-
-    This function fits the T Model incrementally to a set of modelled plants,
-    given a time series of GPP estimates.
-
-    Args:
-        gpp: An array of GPP values
-        d_init: An array of starting diameters
-        traits: Traits to be used
-        time_axis: An axis in P0 and d that represents an annual time series
-        outvars: A list of Tree properties to store.
-
-    Returns:
-        A dictionary of estimates for the time series, exporting the values
-        specified in `outvars`
-    """
-
-    # The gpp array should contain a time axis to increment over. The d_init input
-    # should then be the same shape as P0 _without_ that time axis dimension
-    # and the loop will iterate over the years
-
-    gpp_shape = gpp.shape
-    if time_axis < 0 or time_axis >= len(gpp_shape):
-        raise RuntimeError(f"time_axis must be >= 0 and <= {len(gpp_shape) - 1}")
-
-    # Check that the input shapes for a single year match the shape of the
-    # initial diameters
-    single_year_gpp = np.take(gpp, indices=0, axis=time_axis)
-    _ = check_input_shapes(single_year_gpp, d_init)
-
-    # TODO: - handle 1D GPP time series applied to more than one diameter
-
-    # Initialise the Tree object
-    tree = TTree(traits)
-
-    # Check the requested outvars
-    if "diameter" not in outvars:
-        raise RuntimeWarning("output_vars must include diameter")
-
-    badvars = []
-    for var in outvars:
-
-        try:
-            _ = getattr(tree, var)
-        except AttributeError:
-            badvars.append(var)
-
-    if badvars:
-        raise RuntimeError(f"Unknown tree properties in outvars: {', '.join(badvars)}")
-
-    # Create an array to store the requested variables by adding a dimension
-    # to the gpp input with length set to the number of variables
-    output_shape = gpp_shape + tuple([len(outvars)])
-    output = np.zeros(output_shape)
-
-    # Insert the initial diameters
-    tree.set_diameter(d_init)
-
-    # Create an indexing object to insert values into the output. This is
-    # a bit obscure: the inputs have a time axis and an arbitrary number
-    # of other dimensions and the output adds another dimension for the
-    # output variables. So this object creates a slice (:) on _all_ dimensions
-    # and the loop then replaces the time axis and variable axis with integers.
-    output_index = [slice(None)] * output.ndim
-
-    # Loop over the gpp time axis
-    for year in np.arange(gpp_shape[time_axis]):
-
-        # Calculate the growth based on the current year of gpp
-        tree.calculate_growth(np.take(gpp, indices=year, axis=time_axis))
-
-        # Store the requested variables into the output array
-        for var_idx, each_var in enumerate(outvars):
-
-            # Extract variable values from tree into output - set the last index
-            # (variable dimension) to the variable index and the time axis to the year
-            output_index[-1] = var_idx
-            output_index[time_axis] = year
-            output[tuple(output_index)] = getattr(tree, each_var)
+    outvars: tuple[str, ...] = ("diameter", "height", "crown_area", "delta_d"),
+) -> dict[str, np.ndarray]:
+    """Fit a growth time series using the T Model."""
+    raise NotImplementedError()
+
+
+#     This function fits the T Model incrementally to a set of modelled plants,
+#     given a time series of GPP estimates.
+
+#     Args:
+#         gpp: An array of GPP values
+#         d_init: An array of starting diameters
+#         traits: Traits to be used
+#         time_axis: An axis in P0 and d that represents an annual time series
+#         outvars: A list of Tree properties to store.
+
+#     Returns:
+#         A dictionary of estimates for the time series, exporting the values
+#         specified in `outvars`
+#     """
+
+#     # The gpp array should contain a time axis to increment over. The d_init input
+#     # should then be the same shape as P0 _without_ that time axis dimension
+#     # and the loop will iterate over the years
+
+#     gpp_shape = gpp.shape
+#     if time_axis < 0 or time_axis >= len(gpp_shape):
+#         raise RuntimeError(f"time_axis must be >= 0 and <= {len(gpp_shape) - 1}")
+
+#     # Check that the input shapes for a single year match the shape of the
+#     # initial diameters
+#     single_year_gpp = np.take(gpp, indices=0, axis=time_axis)
+#     _ = check_input_shapes(single_year_gpp, d_init)
+
+#     # TODO: - handle 1D GPP time series applied to more than one diameter
+
+#     # Initialise the Tree object
+#     tree = TTree(d_init, traits)
+
+#     # Check the requested outvars
+#     if "diameter" not in outvars:
+#         raise RuntimeWarning("output_vars must include diameter")
+
+#     badvars = []
+#     for var in outvars:
+
+#         try:
+#             _ = getattr(tree, var)
+#         except AttributeError:
+#             badvars.append(var)
+
+# if badvars:
+#     raise RuntimeError(
+#         f"Unknown tree properties in outvars: {', '.join(badvars)}"
+#         )
+
+#     # Create an array to store the requested variables by adding a dimension
+#     # to the gpp input with length set to the number of variables
+#     output = {v: np.zeros(gpp.shape) for v in outvars}
+
+#     # Create an indexing object to insert values into the output. This is
+#     # a bit obscure: the inputs have a time axis and an arbitrary number
+#     # of other dimensions and the output adds another dimension for the
+#     # output variables. So this object creates a slice (:) on _all_ dimensions
+#     # and the loop then replaces the time axis and variable axis with integers.
+#     output_index = [slice(None)] * gpp.ndim
+
+#     # Loop over the gpp time axis
+#     for year in np.arange(gpp_shape[time_axis]):
+
+#         # Calculate the growth based on the current year of gpp
+#         tree.calculate_growth(np.take(gpp, indices=year, axis=time_axis))
+
+#         # Store the requested variables into the output arrays
+#         for each_var in outvars:
+
+#             # Extract variable values from tree into output - set the last index
+#             # (variable dimension) to the variable index and the time axis to the year
+#             output_index[time_axis] = year
+#             output[each_var][tuple(output_index)] = getattr(tree, each_var)
 
-        # Now update the tree object
-        tree.set_diameter(tree.diameter + getattr(tree, "delta_d"))
+#         # Now update the tree object
+#         tree.reset_diameters(tree.diameter + getattr(tree, "delta_d"))
 
-    return output
+#     return output
```

### Comparing `pyrealm-0.8.1/setup.py` & `pyrealm-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['pyrealm']
+['pyrealm', 'pyrealm.constants', 'pyrealm.pmodel', 'pyrealm_build_data']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Bottleneck>=1.3.5,<2.0.0',
  'dacite>=1.6.0,<2.0.0',
- 'enforce-typing>=1.0.0,<2.0.0',
  'numpy>=1.16.5,<2.0.0',
  'scipy>=1.7.3,<2.0.0',
  'tabulate>=0.8.10,<0.9.0']
 
 setup_kwargs = {
     'name': 'pyrealm',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Python implementations of REALM models',
-    'long_description': '# The `pyrealm` package\n\nThese are development notes for the package, user documentation can be found at:\n\n[](https://pyrealm.readthedocs.io/)\n\n## Overview\n\nThis a Python 3 package intended to provide a common framework for a number of\nrelated models of plant productivity, growth and demography.\n\n## Code development\n\nThe codebase is developed in `git` with a repository at:\n\n[https://github.com/davidorme/pyrealm](https://github.com/davidorme/pyrealm)\n\nIt uses the `git flow` model for development and release. Briefly:\n\n* All code development should happen on the general `develop` branch or on specific\n  `feature/feature_name` branches.\n* Candidate release versions should be made on specific `release/x.y.z` branches\n  and these are then committed to the `master` branch only after final checking.\n* The `master` branch should only ever contain commits representing new release\n  versions - do not work on the `master` branch.\n\n## Continuous integration\n\nThe project uses continuous integration on the Travis platform to check that the\npackage is building correctly as changes are committed to Github. The status of\nbuilds can be seen at:\n\n[https://travis-ci.com/github/davidorme/pyrealm](https://travis-ci.com/github/davidorme/pyrealm)\n\n## Documentation\n\nThe `pyrealm` package is documented using `sphinx`, with source material in the\n`source` directory.\n\nThe documentation in `source` uses [Myst Markdown](https://myst-parser.readthedocs.io/en/latest/)\nrather than the standard `sphinx` reStructuredText (`.rst`) format. This is\nbecause the documentation uses the `myst_nb` extension to `sphinx` that supports\nrunning documentation as a Jupyter notebook: the built documentation includes\nexamples of running code and output plots to demonstrate the use and behaviour\nof the package.\n\nThe `sphinx` configuration includes the `sphinx.ext.mathjax`\nextension to support mathematical notation. This has been configured to also\nload the `mhchem` extension, supporting the rendering of chemical notation.\n\n### Docstrings\n\nThe module codes uses docstrings written in the\n[Google style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).\nUnlike the main documentation pages, the docstrings in code are written using\nreStructuredText because the `autodoc` functions in `sphinx` currently rely on `rst`\ninputs. This allows the function documentation to be stored alongside the code\nand included simply into the documentation.\n\n### Building the documentation\n\nAdditional python packages given in `source/requirements.txt` are needed\nto build the documentation. To actually build the documentation, use\n`make` in the package root, which will use the `Makefile` created by\n`sphinx-quickstart`.\n\n```bash\nmake html\n```\n\n### Online documentation\n\nTODO - change this to github deployment?\n\nThe documentation for the package is hosted at:\n\n[](https://pyrealm.readthedocs.io/en/develop/pmodel.html)\n\nThis has been configured to build commits to the `master` branch, which should\ngenerate version specific sets of documentation.\n\n### Referencing\n\nThe documentation uses the `sphinxcontrib-bibtex` package to support citations.\nThis uses Latex like citation keys in the documentation to insert references and\nbuild a bibliography. The reference library in `source/refs.bib` needs to be\nkept up to date with the literature for the project.\n\nAt present, that package uses a rather ugly citation style. I\'m hoping the\n`sphinx_astrorefs` package will help out, but there is currently an issue\ngetting that package to load.\n\n## Testing\n\n### Developer installation\n\nUse the local directory as an editable installation of the package\n\n```sh\npip install -e .\n```\n\n### Using `doctest`\n\nThe package docstrings contain `doctest` examples of code use. These are\nintended to demonstrate use and to validate a reference set of inputs against\nexpected outputs. They do not provide extensive unit testing! To run the\ndocstring tests, use:\n\n```bash\npython -m doctest pyrealm/pmodel.py\npython -m doctest pyrealm/*.py\n```\n\nFor `doctest` on warnings, see the example for `pyrealm.utilities.convert_rh_to_vpd`\nwhich redirects the stderr to stdout to allow for the warning text to be\nincluded in the doctest.\n\n### Using `pytest`\n\nThe `test` directory contains `pytest` modules to provide greater testing of\ndifferent input combinations (scalars and arrays) and to check errors are\nraised correctly.\n\n```bash\npytest\n```\n\n### Reference values for testing\n\nThe sources of the reference inputs and outputs are:\n\n`pmodel` module:\n    Benjamin Stocker\'s [`rpmodel`](https://github.com/stineb/rpmodel/tree/master/R)\n    implementation of the P-model in R. The `test` directory contains a YAML\n    file of inputs (`test_inputs.yaml`) and an `R` script (`test_output_rpmodel.R`)\n    that are used to generate a larger YAML file (`test_outputs_rpmodel.R`) that\n    are loaded and validated against {mod}`pyrealm.pmodel` by `test_pmodel.py`.\n\n## Continuous Integration\n\n## Git flow\n\n### Configure `git`\n\nIt is easier if `git` is configured to push new tags along with commits. This\nessentially just means that new releases can be sent with a single commit,\nwhich is simpler and saves Travis from building both the the code commit and\nthen the tagged version. This only needs to be set once.\n\n```bash\nset git config --global push.followTags true\n```\n\nUsing git-flow and travis\n\nUse git flow to create a release\n\n```bash\ngit flow release start 0.3.0\n```\n\nand then bump the version number in `version.py`.\n\nCheck the package builds and installs locally:\n\n```bash\npython setup.py sdist bdist_wheel\n```\n\nCommit the version number change and then publish the branch:\n\n```sh\ngit commit -m "Version bump" pyrealm/version.py\ngit flow release publish x.y.z\n```\n\nto get the branch onto the origin repository and hence into Travis.\n\n### Use twine to check it passes onto testpypi\n\nWe are using `twine` to publish versions to PyPi, and using the `testpypi`\nsandbox to check release candidates are accepted. This needs an account\nfor both pypi and testpypi.\n\nRemembering to change the version number, use `twine` to upload the built\nversions to the `testpypi` site:\n\n```sh\ntwine upload -r testpypi dist/*x.y.z*\n```\n\n### Check the documentation builds\n\nLog in to:\n\n[](https://readthedocs.org)\n\nwhich is the admin site controlling the build process. From the Versions\ntab, activate the `release/x.y.z` branch and wait for it to build. Check\nthe Builds tab to see that it has built successfully and maybe check\nupdates! If it has built succesfully, then go back to the Versions tab\nand deactivate and hide the branch.\n\n## Success\n\nOnce all seems well,  the next step is to finish the release, which merges\nchanges into `develop` and into a tagged commit on `master`. You then need\nto checkout the master branch and push the new version and tag to GitHub.\n\n```bash\ngit flow release finish x.y.z\ngit checkout master\ngit push\n```\n\n## PyPi upload\n\nTo upload the new version to the main PyPi site, run the build process again\nin the `master` branch to get the release builds:\n\n```sh\npython setup.py sdist bdist_wheel\n```\n\nAnd then release the distribution using `twine` for use via `pip` - this time\nnot using the `testpypi` sandbox.\n\n```sh\ntwine upload dist/*x.y.z*\n```\n\nNow:\n\n* **switch back to `develop`!**\n\n```sh\ngit checkout develop\n```\n\n* Bump the version number to add `.post9000` to show the code is in development again.\n',
+    'long_description': '# The `pyrealm` package\n\nThese are development notes for the package, user documentation can be found at:\n\n[](https://pyrealm.readthedocs.io/)\n\n## Overview\n\nThis a Python 3 package intended to provide a common framework for a number of\nrelated models of plant productivity, growth and demography.\n\n## Code development\n\n### Package managment\n\nThe package uses `poetry` to manage dependencies, generate virtual environments for code\ndevelopment and then for package building and publication. You will need to install\n`poetry` to develop the code.\n\n### Source code management\n\nThe codebase is developed in `git` with a repository at:\n\n[](https://github.com/davidorme/pyrealm)\n\nIt uses the `git flow` model for development and release. Briefly:\n\n* All code development should happen specific `feature/feature_name` branches.\n* Pull requests (PR) should be made to merge feature branches into the `develop` branch.\n* Candidate release versions should be made on specific `release/x.y.z` branches\n  and these are then committed to the `master` branch only after final checking.\n* The `master` branch should only ever contain commits representing new release\n  versions - do not work on the `master` branch.\n\nBoth the `develop` and `master` branches are protected on GitHub to avoid accidents!\n\n### Code quality\n\nThe project uses the `pre-commit` tool to enforce code quality. The configuration file\n`.pre-commit-config.yaml` shows the details of the tool chain, but `isort`, `black`,\n`flake8` and `markdownlint` are used to maintain code quality. You will need to install\n`pre-commit` to develop package code, and each PR must pass the same set of checks.\n\n### Code testing\n\n#### Using `doctest`\n\nThe package docstrings contain `doctest` examples of code use. These are intended to\ndemonstrate use and to validate a reference set of inputs against expected outputs. They\ndo not provide extensive unit testing! To run the docstring tests, use:\n\n```bash\npython -m doctest pyrealm/pmodel.py\npython -m doctest pyrealm/*.py\n```\n\nFor `doctest` on warnings, see the example for `pyrealm.utilities.convert_rh_to_vpd`\nwhich redirects the stderr to stdout to allow for the warning text to be included in the\ndoctest.\n\n#### Using `pytest`\n\nThe `test` directory contains `pytest` modules to provide greater testing of different\ninput combinations and to check errors are raised correctly. These are the main tests\nthat the package is behaving as expected.\n\n```bash\npytest\n```\n\n### Continuous integration\n\nThe project uses continuous integration via GitHub Actions to check that the package is\nbuilding correctly and that both `doctest` and `pytest` tests are passing. The status of\nbuilds can be seen at:\n\n[](https://github.com/davidorme/pyrealm/actions)\n\n## Documentation\n\nThe `pyrealm` package is documented using `sphinx`, with source material in the\n`docs/source` directory.\n\nThe documentation in `source` uses [Myst\nMarkdown](https://myst-parser.readthedocs.io/en/latest/) rather than the standard\n`sphinx` reStructuredText (`.rst`) format. This is because the documentation uses the\n`myst_nb` extension to `sphinx` that supports running documentation as a Jupyter\nnotebook: the built documentation includes examples of running code and output plots to\ndemonstrate the use and behaviour of the package.\n\nThe `sphinx` configuration includes the `sphinx.ext.mathjax` extension to support\nmathematical notation. This has been configured to also load the `mhchem` extension,\nsupporting the rendering of chemical notation.\n\n### Docstrings\n\nThe module codes uses docstrings written in the [Google\nstyle](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).\nUnlike the main documentation pages, the docstrings in code are written using\nreStructuredText because the `autodoc` functions in `sphinx` currently rely on `rst`\ninputs. This allows the function documentation to be stored alongside the code and\nincluded simply into the documentation.\n\n### Building the documentation\n\nAdditional python packages given in `docs/source/requirements.txt` are needed to build\nthe documentation. To actually build the documentation, use `make` in the package root,\nwhich will use the `Makefile` created by `sphinx-quickstart`.\n\n```bash\ncd docs\nmake html\n```\n\n### Online documentation\n\nThe documentation for the package is hosted at:\n\n[](https://pyrealm.readthedocs.io/en/develop/pmodel.html)\n\nThis has been configured to build commits to the `master` branch, which should\ngenerate version specific sets of documentation.\n\n### Referencing\n\nThe documentation uses the `sphinxcontrib-bibtex` package to support citations.\nThis uses Latex like citation keys in the documentation to insert references and\nbuild a bibliography. The reference library in `source/refs.bib` needs to be\nkept up to date with the literature for the project. The `sphinx_astrorefs` package is\nused to provide an Author Date style citation format.\n\n## Release process\n\nReleasing a new version of the package follows the flow below:\n\n1. Create a `release` branch from `develop` containing the new release code.\n2. Check that this branch builds correctly, that the documentation builds correctly and\n   that the package publishes to the `test-pypi` repository.\n3. When all is well, create pull requests on GitHub to merge the `release` branch into\n   both `develop` and `master`, along with a version tag for the release.\n4. Once you have updated your local repository, then the tag can be used to build and\n   publish the final version to the main PyPi site.\n\nIt is easier if `git` is configured to push new tags along with commits. This\nessentially just means that new releases can be sent with a single commit. This only\nneeds to be set once.\n\n```bash\nset git config --global push.followTags true\n```\n\n### Create the release branch\n\nUsing `git flow` commands as an example to create a new release:\n\n```sh\ngit flow release start new_release\n```\n\nObviously, use something specific, not `new_release`! Ideally, you would do a dry run of\nthe next step and use the version - but it should be fairly obvious what this will be!\n\nThe `poetry version` command can then be used to bump the version number. Note that the\ncommand needs a \'bump rule\', which sets which part of the semantic version number to\nincrement (`major`, `minor` or `patch`). For example:\n\n```sh\npoetry version patch\n```\n\nThis updates `pyproject.toml`. At present, the package is set up so that you also *have\nto update the version number in `pyrealm/version.py`* to match manually.\n\n### Publish and test the release branch\n\nWith those changes committed, publish the release branch:\n\n```sh\ngit commit -m "Version bump" pyrealm/version.py\ngit flow release publish new_release\n```\n\nThe GitHub Actions will then ensure that the code passes quality assurance and then runs\nthe test suites on a range of Python versions and operating systems.\n\n### Check package publication\n\nThe `sdist` and `wheel` builds for the package can then be built locally using `poetry`\n\n```bash\npoetry build\n```\n\nThe first time this is run, `poetry` needs to be configured to add the Test PyPi\nrepository and an API token from that site. Note that accounts are not shared between\nthe Test and main PyPi sites: the API token for `test-pypi` is different from\n`pypi` and you have to log in to each system separately and generate a token on each.\n\n```sh\npoetry config repositories.test-pypi https://test.pypi.org/legacy/\npoetry config pypi-token.test-pypi <your-token>\n```\n\nThe built packages can then be published to `test-pypi` using:\n\n```sh\npoetry publish -r test-pypi\n```\n\n### Check the documentation builds\n\nLog in to:\n\n[](https://readthedocs.org)\n\nwhich is the admin site controlling the build process. From the Versions tab, activate\nthe `release/new_release` branch and wait for it to build. Check the Builds tab to see\nthat it has built successfully and maybe check updates! If it has built succesfully, do\ncheck pages to make sure that page code has executed successfully, and then go back to\nthe Versions tab and deactivate and hide the branch.\n\n### Create pull requests into `master` and `develop`\n\nIf all is well, then two PRs need to be made on GitHub:\n\n* The `release` branch into `master`, to bring all commits since the last release and\n  any fixes on release into `master`.\n* The `release` branch into `develop`, to bring any `release` fixes back into `develop`.\n\nOnce both of those have been merged, the `feature` branch can be deleted.\n\n### Tag, build and publish\n\nOnce the `origin` repository is merged, then use `git pull` to bring `develop` and\n`master` up to date on a local repo. Then, create a tag using the release version.\n\n```sh\ngit checkout master\ngit tag <version>\ngit push --tags\n```\n\nThe final commit on `master` is now tagged with the release version. You can add tags on\nthe GitHub website, but only by using the GitHub release system and we are using PyPi to\ndistribute package releases.\n\nBefore publishing a package to the main PyPi site for the first time, you need to set an\nAPI token for PyPi.\n\n```sh\npoetry config pypi-token.pypi <your-token>\n```\n\nAnd now you can build the packages from `master` and publish.\n\n```sh\npoetry build\npoetry publish\n```\n',
     'author': 'David Orme',
     'author_email': 'd.orme@imperial.ac.uk',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://pyrealm.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.11',
+    'python_requires': '>=3.9,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pyrealm-0.8.1/PKG-INFO` & `pyrealm-0.9.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pyrealm
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python implementations of REALM models
 Home-page: https://pyrealm.readthedocs.io/
 License: MIT
 Author: David Orme
 Author-email: d.orme@imperial.ac.uk
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: Bottleneck (>=1.3.5,<2.0.0)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
-Requires-Dist: enforce-typing (>=1.0.0,<2.0.0)
 Requires-Dist: numpy (>=1.16.5,<2.0.0)
 Requires-Dist: scipy (>=1.7.3,<2.0.0)
 Requires-Dist: tabulate (>=0.8.10,<0.9.0)
 Project-URL: Repository, https://github.com/davidorme/pyrealm
 Description-Content-Type: text/markdown
 
 # The `pyrealm` package
@@ -34,236 +32,254 @@
 ## Overview
 
 This a Python 3 package intended to provide a common framework for a number of
 related models of plant productivity, growth and demography.
 
 ## Code development
 
+### Package managment
+
+The package uses `poetry` to manage dependencies, generate virtual environments for code
+development and then for package building and publication. You will need to install
+`poetry` to develop the code.
+
+### Source code management
+
 The codebase is developed in `git` with a repository at:
 
-[https://github.com/davidorme/pyrealm](https://github.com/davidorme/pyrealm)
+[](https://github.com/davidorme/pyrealm)
 
 It uses the `git flow` model for development and release. Briefly:
 
-* All code development should happen on the general `develop` branch or on specific
-  `feature/feature_name` branches.
+* All code development should happen specific `feature/feature_name` branches.
+* Pull requests (PR) should be made to merge feature branches into the `develop` branch.
 * Candidate release versions should be made on specific `release/x.y.z` branches
   and these are then committed to the `master` branch only after final checking.
 * The `master` branch should only ever contain commits representing new release
   versions - do not work on the `master` branch.
 
-## Continuous integration
+Both the `develop` and `master` branches are protected on GitHub to avoid accidents!
+
+### Code quality
+
+The project uses the `pre-commit` tool to enforce code quality. The configuration file
+`.pre-commit-config.yaml` shows the details of the tool chain, but `isort`, `black`,
+`flake8` and `markdownlint` are used to maintain code quality. You will need to install
+`pre-commit` to develop package code, and each PR must pass the same set of checks.
+
+### Code testing
 
-The project uses continuous integration on the Travis platform to check that the
-package is building correctly as changes are committed to Github. The status of
+#### Using `doctest`
+
+The package docstrings contain `doctest` examples of code use. These are intended to
+demonstrate use and to validate a reference set of inputs against expected outputs. They
+do not provide extensive unit testing! To run the docstring tests, use:
+
+```bash
+python -m doctest pyrealm/pmodel.py
+python -m doctest pyrealm/*.py
+```
+
+For `doctest` on warnings, see the example for `pyrealm.utilities.convert_rh_to_vpd`
+which redirects the stderr to stdout to allow for the warning text to be included in the
+doctest.
+
+#### Using `pytest`
+
+The `test` directory contains `pytest` modules to provide greater testing of different
+input combinations and to check errors are raised correctly. These are the main tests
+that the package is behaving as expected.
+
+```bash
+pytest
+```
+
+### Continuous integration
+
+The project uses continuous integration via GitHub Actions to check that the package is
+building correctly and that both `doctest` and `pytest` tests are passing. The status of
 builds can be seen at:
 
-[https://travis-ci.com/github/davidorme/pyrealm](https://travis-ci.com/github/davidorme/pyrealm)
+[](https://github.com/davidorme/pyrealm/actions)
 
 ## Documentation
 
 The `pyrealm` package is documented using `sphinx`, with source material in the
-`source` directory.
+`docs/source` directory.
 
-The documentation in `source` uses [Myst Markdown](https://myst-parser.readthedocs.io/en/latest/)
-rather than the standard `sphinx` reStructuredText (`.rst`) format. This is
-because the documentation uses the `myst_nb` extension to `sphinx` that supports
-running documentation as a Jupyter notebook: the built documentation includes
-examples of running code and output plots to demonstrate the use and behaviour
-of the package.
-
-The `sphinx` configuration includes the `sphinx.ext.mathjax`
-extension to support mathematical notation. This has been configured to also
-load the `mhchem` extension, supporting the rendering of chemical notation.
+The documentation in `source` uses [Myst
+Markdown](https://myst-parser.readthedocs.io/en/latest/) rather than the standard
+`sphinx` reStructuredText (`.rst`) format. This is because the documentation uses the
+`myst_nb` extension to `sphinx` that supports running documentation as a Jupyter
+notebook: the built documentation includes examples of running code and output plots to
+demonstrate the use and behaviour of the package.
+
+The `sphinx` configuration includes the `sphinx.ext.mathjax` extension to support
+mathematical notation. This has been configured to also load the `mhchem` extension,
+supporting the rendering of chemical notation.
 
 ### Docstrings
 
-The module codes uses docstrings written in the
-[Google style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+The module codes uses docstrings written in the [Google
+style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 Unlike the main documentation pages, the docstrings in code are written using
 reStructuredText because the `autodoc` functions in `sphinx` currently rely on `rst`
-inputs. This allows the function documentation to be stored alongside the code
-and included simply into the documentation.
+inputs. This allows the function documentation to be stored alongside the code and
+included simply into the documentation.
 
 ### Building the documentation
 
-Additional python packages given in `source/requirements.txt` are needed
-to build the documentation. To actually build the documentation, use
-`make` in the package root, which will use the `Makefile` created by
-`sphinx-quickstart`.
+Additional python packages given in `docs/source/requirements.txt` are needed to build
+the documentation. To actually build the documentation, use `make` in the package root,
+which will use the `Makefile` created by `sphinx-quickstart`.
 
 ```bash
+cd docs
 make html
 ```
 
 ### Online documentation
 
-TODO - change this to github deployment?
-
 The documentation for the package is hosted at:
 
 [](https://pyrealm.readthedocs.io/en/develop/pmodel.html)
 
 This has been configured to build commits to the `master` branch, which should
 generate version specific sets of documentation.
 
 ### Referencing
 
 The documentation uses the `sphinxcontrib-bibtex` package to support citations.
 This uses Latex like citation keys in the documentation to insert references and
 build a bibliography. The reference library in `source/refs.bib` needs to be
-kept up to date with the literature for the project.
-
-At present, that package uses a rather ugly citation style. I'm hoping the
-`sphinx_astrorefs` package will help out, but there is currently an issue
-getting that package to load.
-
-## Testing
-
-### Developer installation
+kept up to date with the literature for the project. The `sphinx_astrorefs` package is
+used to provide an Author Date style citation format.
 
-Use the local directory as an editable installation of the package
+## Release process
 
-```sh
-pip install -e .
-```
+Releasing a new version of the package follows the flow below:
 
-### Using `doctest`
+1. Create a `release` branch from `develop` containing the new release code.
+2. Check that this branch builds correctly, that the documentation builds correctly and
+   that the package publishes to the `test-pypi` repository.
+3. When all is well, create pull requests on GitHub to merge the `release` branch into
+   both `develop` and `master`, along with a version tag for the release.
+4. Once you have updated your local repository, then the tag can be used to build and
+   publish the final version to the main PyPi site.
 
-The package docstrings contain `doctest` examples of code use. These are
-intended to demonstrate use and to validate a reference set of inputs against
-expected outputs. They do not provide extensive unit testing! To run the
-docstring tests, use:
+It is easier if `git` is configured to push new tags along with commits. This
+essentially just means that new releases can be sent with a single commit. This only
+needs to be set once.
 
 ```bash
-python -m doctest pyrealm/pmodel.py
-python -m doctest pyrealm/*.py
+set git config --global push.followTags true
 ```
 
-For `doctest` on warnings, see the example for `pyrealm.utilities.convert_rh_to_vpd`
-which redirects the stderr to stdout to allow for the warning text to be
-included in the doctest.
+### Create the release branch
 
-### Using `pytest`
+Using `git flow` commands as an example to create a new release:
 
-The `test` directory contains `pytest` modules to provide greater testing of
-different input combinations (scalars and arrays) and to check errors are
-raised correctly.
-
-```bash
-pytest
+```sh
+git flow release start new_release
 ```
 
-### Reference values for testing
+Obviously, use something specific, not `new_release`! Ideally, you would do a dry run of
+the next step and use the version - but it should be fairly obvious what this will be!
 
-The sources of the reference inputs and outputs are:
+The `poetry version` command can then be used to bump the version number. Note that the
+command needs a 'bump rule', which sets which part of the semantic version number to
+increment (`major`, `minor` or `patch`). For example:
 
-`pmodel` module:
-    Benjamin Stocker's [`rpmodel`](https://github.com/stineb/rpmodel/tree/master/R)
-    implementation of the P-model in R. The `test` directory contains a YAML
-    file of inputs (`test_inputs.yaml`) and an `R` script (`test_output_rpmodel.R`)
-    that are used to generate a larger YAML file (`test_outputs_rpmodel.R`) that
-    are loaded and validated against {mod}`pyrealm.pmodel` by `test_pmodel.py`.
-
-## Continuous Integration
+```sh
+poetry version patch
+```
 
-## Git flow
+This updates `pyproject.toml`. At present, the package is set up so that you also *have
+to update the version number in `pyrealm/version.py`* to match manually.
 
-### Configure `git`
+### Publish and test the release branch
 
-It is easier if `git` is configured to push new tags along with commits. This
-essentially just means that new releases can be sent with a single commit,
-which is simpler and saves Travis from building both the the code commit and
-then the tagged version. This only needs to be set once.
+With those changes committed, publish the release branch:
 
-```bash
-set git config --global push.followTags true
+```sh
+git commit -m "Version bump" pyrealm/version.py
+git flow release publish new_release
 ```
 
-Using git-flow and travis
+The GitHub Actions will then ensure that the code passes quality assurance and then runs
+the test suites on a range of Python versions and operating systems.
 
-Use git flow to create a release
+### Check package publication
 
-```bash
-git flow release start 0.3.0
-```
-
-and then bump the version number in `version.py`.
-
-Check the package builds and installs locally:
+The `sdist` and `wheel` builds for the package can then be built locally using `poetry`
 
 ```bash
-python setup.py sdist bdist_wheel
+poetry build
 ```
 
-Commit the version number change and then publish the branch:
+The first time this is run, `poetry` needs to be configured to add the Test PyPi
+repository and an API token from that site. Note that accounts are not shared between
+the Test and main PyPi sites: the API token for `test-pypi` is different from
+`pypi` and you have to log in to each system separately and generate a token on each.
 
 ```sh
-git commit -m "Version bump" pyrealm/version.py
-git flow release publish x.y.z
+poetry config repositories.test-pypi https://test.pypi.org/legacy/
+poetry config pypi-token.test-pypi <your-token>
 ```
 
-to get the branch onto the origin repository and hence into Travis.
-
-### Use twine to check it passes onto testpypi
-
-We are using `twine` to publish versions to PyPi, and using the `testpypi`
-sandbox to check release candidates are accepted. This needs an account
-for both pypi and testpypi.
-
-Remembering to change the version number, use `twine` to upload the built
-versions to the `testpypi` site:
+The built packages can then be published to `test-pypi` using:
 
 ```sh
-twine upload -r testpypi dist/*x.y.z*
+poetry publish -r test-pypi
 ```
 
 ### Check the documentation builds
 
 Log in to:
 
 [](https://readthedocs.org)
 
-which is the admin site controlling the build process. From the Versions
-tab, activate the `release/x.y.z` branch and wait for it to build. Check
-the Builds tab to see that it has built successfully and maybe check
-updates! If it has built succesfully, then go back to the Versions tab
-and deactivate and hide the branch.
-
-## Success
-
-Once all seems well,  the next step is to finish the release, which merges
-changes into `develop` and into a tagged commit on `master`. You then need
-to checkout the master branch and push the new version and tag to GitHub.
+which is the admin site controlling the build process. From the Versions tab, activate
+the `release/new_release` branch and wait for it to build. Check the Builds tab to see
+that it has built successfully and maybe check updates! If it has built succesfully, do
+check pages to make sure that page code has executed successfully, and then go back to
+the Versions tab and deactivate and hide the branch.
 
-```bash
-git flow release finish x.y.z
-git checkout master
-git push
-```
+### Create pull requests into `master` and `develop`
 
-## PyPi upload
+If all is well, then two PRs need to be made on GitHub:
 
-To upload the new version to the main PyPi site, run the build process again
-in the `master` branch to get the release builds:
+* The `release` branch into `master`, to bring all commits since the last release and
+  any fixes on release into `master`.
+* The `release` branch into `develop`, to bring any `release` fixes back into `develop`.
 
-```sh
-python setup.py sdist bdist_wheel
-```
+Once both of those have been merged, the `feature` branch can be deleted.
+
+### Tag, build and publish
 
-And then release the distribution using `twine` for use via `pip` - this time
-not using the `testpypi` sandbox.
+Once the `origin` repository is merged, then use `git pull` to bring `develop` and
+`master` up to date on a local repo. Then, create a tag using the release version.
 
 ```sh
-twine upload dist/*x.y.z*
+git checkout master
+git tag <version>
+git push --tags
 ```
 
-Now:
+The final commit on `master` is now tagged with the release version. You can add tags on
+the GitHub website, but only by using the GitHub release system and we are using PyPi to
+distribute package releases.
 
-* **switch back to `develop`!**
+Before publishing a package to the main PyPi site for the first time, you need to set an
+API token for PyPi.
 
 ```sh
-git checkout develop
+poetry config pypi-token.pypi <your-token>
 ```
 
-* Bump the version number to add `.post9000` to show the code is in development again.
+And now you can build the packages from `master` and publish.
+
+```sh
+poetry build
+poetry publish
+```
```

