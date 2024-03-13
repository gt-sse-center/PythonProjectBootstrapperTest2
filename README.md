# PythonProjectBootstrapperTest2

[![CI](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions/workflows/standard.yaml/badge.svg?event=push)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions/workflows/standard.yaml)
[![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/davidbrownell/2f9d770d13e3a148424f374f74d41f4b/raw/PythonProjectBootstrapperTest2_coverage.json)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions)
[![License](https://img.shields.io/github/license/gt-sse-center/PythonProjectBootstrapperTest2?color=dark-green)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/blob/master/LICENSE.txt)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/y/gt-sse-center/PythonProjectBootstrapperTest2?color=dark-green)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/commits/main/)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PythonProjectBootstrapperTest2?color=dark-green)](https://pypi.org/project/pythonprojectbootstrappertest2/)
[![PyPI - Version](https://img.shields.io/pypi/v/PythonProjectBootstrapperTest2?color=dark-green)](https://pypi.org/project/pythonprojectbootstrappertest2/)
[![PyPI - Downloads](https://img.shields.io/pypi/dm/PythonProjectBootstrapperTest2)](https://pypistats.org/packages/pythonprojectbootstrappertest2)

[![Code Coverage (BugBug)](https://img.shields.io/endpoint?url=https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/releases/latest/download/__code_coverage_badge_info.json)](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/actions)



# PythonProjectBootstrapperTest2
Testing output produced by PythonProjectBootstrapper

### Overview

TODO: Complete this section

### How to use PythonProjectBootstrapperTest2

TODO: Complete this section

## Installation via Executable

Download an executable for Linux, MacOS, or Windows to use the functionality provided by this repository without a dependency on [Python](https://www.python.org).

1. Download the archive for the latest release [here](https://github.com/gt-sse-center/PythonProjectBootstrapperTest2/releases/latest); the files will begin with `exe.` and contain the name of your operating system.
2. Decompress the archive

## Installation via pip

Install the PythonProjectBootstrapperTest2 package via [pip](https://pip.pypa.io/en/stable/) (Package Installer for Python) to use it with your python code.

`pip install PythonProjectBootstrapperTest2`

## Local Development

Follow these steps to prepare the repository for local development activities.

1) Clone this repository
2) Bootstrap the local repository by running...
    | Operating System | Command |
    | --- | --- |
    | Linux / MacOS | <p>Standard:<br/>`Bootstrap.sh`</p><p>Standard + packaging:<br/>`Bootstrap.sh --package`</p> |
    | Windows | <p>Standard:<br/>`Bootstrap.cmd`</p><p>Standard + packaging:<br/>`Bootstrap.cmd --package`</p> |
3) Activate the development environment by running...
    | Operating System | Command |
    | --- | --- |
    | Linux / MacOS | `. ./Activate.sh` |
    | Windows | `Activate.cmd` |
4) Invoke `Build.py`
    | Command | Description | Example | Notes |
    | --- | --- | --- | --- |
    | `black` | Validates that the source code is formatted by [black](https://github.com/psf/black). | <p>Validation:<br/>`python Build.py black`</p><p>Perform formatting:<br/>`python Build.py black --format`</p> | |
    | `pylint` | Validates the source code using [pylint](https://github.com/pylint-dev/pylint). | `python Build.py pylint` | |
    | `pytest` | Runs automated tests using [pytest](https://docs.pytest.org/). | <p>Without Code Coverage:<br/>`python Build.py pytest`</p><p>With Code Coverage:<br/>`python Build.py pytest --code-coverage`</p> | |
    | `update_version` | Updates the [semantic version](https://semver.org/) of the package based on git commits using [AutoGitSemVer](https://github.com/davidbrownell/AutoGitSemVer). | `python Build.py update_version` | |
    | `package` | Creates a Python wheel package for distribution; outputs to the `/dist` directory. | `python Build.py package` | Requires `--package` when bootstrapping in step #2. |
    | `publish` | Publishes a Python wheel package to [PyPi](https://pypi.org/). | <p>https://test.pypi.org:<br/>`python Build.py publish`</p><p>https://pypi.org:<br/>`python Build.py publish --production`</p> | Requires `--package` when bootstrapping in step #2. |
    | `build_binary` | Builds an executable for your package that can be run on machines without a python installation; outputs to the `/build` directory. | `python Build.py build_binary` | Requires `--package` when bootstrapping in step #2. |
    | `create_docker_image` | Creates a [Docker](https://www.docker.com/) image based on the current development environment. This supports the "Reusable" aspect of [FAIR principles](https://www.go-fair.org/fair-principles/) by creating a snapshot of the repository and all of its dependencies as they exist in a single moment in time. | `python Build.py create_docker_image` | Requires docker. |


5) [Optional] Deactivate the development environment by running...
    | Operating System | Command |
    | --- | --- |
    | Linux / MacOS | `. ./Deactivate.sh` |
    | Windows | `Deactivate.cmd` |

## License

PythonProjectBootstrapperTest2 is licensed under the <a href="https://choosealicense.com/licenses/mit/" target="_blank">MIT</a> license.
