# Cookiecutter Hipster PyPackage

Cookiecutter template for a cutting-edge Python package: Hatch, ruff, mypy, GitHub Actions and more!

## Features

* [X] Lightweight starter
* [X] [Hatch](https://hatch.pypa.io/latest/install/) package management
* [X] Linting and formatting with [`ruff`](https://github.com/charliermarsh/ruff) and [`black`](https://github.com/psf/black)
* [X] Type checking with [`mypy`](https://github.com/python/mypy)
* [X] Unit tests with [`pytest`](https://github.com/pytest-dev/pytest)
* [X] Documentation with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) and docstring reference support with [mkdocstrings](https://mkdocstrings.github.io/).
* [X] Ready-to-use [GitHub Actions](https://help.github.com/en/actions/automating-your-workflow-with-github-actions) pipelines

## Quickstart

Generate the project:

```bash
cookiecutter https://github.com/frankie567/cookiecutter-hipster-pypackage
```

The generator will automatically call `hatch env create` at the end.

Then, for the GitHub Actions pipelines to work correctly, you should:

* Enable the GitHub repository in Codecov
* Set `CODECOV_TOKEN` in your GitHub repository secrets. Uou can find in the Codecov settings of the corresponding project
* [Create a token](https://pypi.org/help/#apitoken) for your PyPI account and set the following secrets:
    * `HATCH_INDEX_USER`: `__token__`
    * `HATCH_INDEX_AUTH`: Your API token

## License

This project is licensed under the terms of the MIT license.
