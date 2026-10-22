# Smarty template engine
Smarty is a template engine for PHP, facilitating the separation of presentation (HTML/CSS) from application logic. 

![CI](https://github.com/smarty-php/smarty/workflows/CI/badge.svg)

## Documentation
Read the [documentation](https://smarty-php.github.io/smarty/) to find out how to use it. 

## Requirements
Smarty can be run with PHP 8.3 to PHP 8.5.

## Installation
Smarty versions 3.1.11 or later can be installed with [Composer](https://getcomposer.org/).

To get the latest stable version of Smarty use:
```bash
composer require smarty/smarty
````

More in the [Getting Started](./docs/getting-started.md) section of the docs.

## Secret check (optional, local)

This repository ships an optional [pre-commit](https://pre-commit.com) hook that runs [gitleaks](https://github.com/gitleaks/gitleaks) to catch secrets before they are committed:

```sh
pip install pre-commit && pre-commit install
```

The check only runs on the developer machine. It does not run in CI and does not block anything there. Server-side GitHub push protection remains the hard gate.
