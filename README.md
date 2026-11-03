# IBM DevOps Capstone Project

[![Build Status](https://github.com/anushkashelare-dev/devops-capstone-project/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/anushkashelare-dev/devops-capstone-project/actions/workflows/build.yml)

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python 3.9](https://img.shields.io/badge/Python-3.9-green.svg)](https://shields.io/)

This repository contains the IBM DevOps Capstone Project: an Account microservice built with Python and Flask. The project focuses on implementing and testing REST API operations and automating build validation with GitHub Actions.

## Development environment

The original project labs are designed for the IBM Skills Network Cloud IDE with OpenShift. See the course instructions for the complete environment setup.

For local development, install the dependencies with:

```bash
python -m pip install -r requirements.txt
```

Run lint checks with:

```bash
make lint
```

Run the unit tests with a PostgreSQL database available and configured through `DATABASE_URI`:

```bash
make tests
```

## Project layout

- `service/` — Flask account service, models, configuration, and REST routes.
- `tests/` — unit tests for the service.
- `tekton/` — Tekton pipeline resources.
- `.github/workflows/build.yml` — GitHub Actions build workflow.

## Build

The build workflow runs on pushes and pull requests to `main`. It installs the Python dependencies, runs Flake8 lint checks, and executes the unit test suite against PostgreSQL.

## License

Licensed under the Apache License 2.0. See [LICENSE](LICENSE).
