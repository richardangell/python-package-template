# python-package-template

Template project for Python packages.

The package name in this repo is `package` which needs to be updated.

## Environment set up

Create the python environment using [pipenv](https://pipenv.pypa.io/en/latest/). [pyenv](https://github.com/pyenv/pyenv) or [pyenv-win](https://github.com/pyenv-win/pyenv-win) may also be needed if the required version of Python is not available.

To create the current envionrment specified in the `Pipfile` run;

`pipenv install`

## Project contents

### Github actions

Github action scripts to run the following 
- `coverage` over `pytest`
- `pre-commit`
- `tox`
- check that the `_version.py` is modified on pull requests

### Source code

- top level `__init__.py`
- `_version.py` script for version number

### Tests

- empty `conftest.py` script in the `tests` folder

### Other configuration

- `.coveragerc` configuration
- `.flake8` configuration
- `.gitignore` settings
- `.pre-commit-config.yml` specifying;
  - black
  - flake8
  - mypy
  - bandit
- `bandit.yml` configuration
- `LICENSE` (BSD 3-Clause "New" or "Revised" License)
- `Pipfile` specifying the development environment
- `pyproject.toml` using `flit` as the package build tool
- `tox.ini` configuration
