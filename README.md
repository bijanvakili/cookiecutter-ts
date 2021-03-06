# cookiecutter-ts

Cookiecutter template for Typescript projects.

## Introduction

This will setup a project with:

* Compilers
    * [TypeScript](https://www.typescriptlang.org/)
* Static Analysis (linters)
    * [ESLint](https://eslint.org/) for `.ts` and `.js` files
    * [markdownlint](https://github.com/DavidAnson/markdownlint) for `.md` files
* Code formatters
    * [prettier](https://prettier.io/)
* Git `pre-commit` [hook](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) to run both linters and formatters (read-only)

## Requirements

* [python](https://www.python.org/)

## Instructions

    cd ./cookiecutter-ts
    pip install -r requirements-dev.txt
    # use the parent directory, not the target
    cookiecutter --output-dir /path/to/parent .
## Testing

    cookiecutter --no-input --output-dir /tmp/myparent --config-file ./test-template-params.yaml .
