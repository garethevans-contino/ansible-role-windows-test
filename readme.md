# Documentation

## Purpose

To have a template repository with the minimum required pre-commit hooks ready to ensure developers are able to work without obsticles from security and linting checks but also a customisable platform for them to build on to help improve code quality.

### Technology
We're using Pre-Commit Hooks and configuration from [https://pre-commit.com/](https://pre-commit.com/)

## History

|Version                |Author                          |Changes                         |Date|
|----------------|-------------------------------|-----------------------------|09/11/2020|
|v0.1|Gareth Evans            |Initial Version|

## Under the bonnet/hood

### Security Tools
|Name                |Version                          |URL                         |
|----------------|-------------------------------|-----------------------------|
|**Detect Secrets**|v0.13.0            |https://github.com/Yelp/detect-secrets|

### Linting/Validation Tools
|Name                |Version                          |URL                         |
|----------------|-------------------------------|-----------------------------|
|**YAML Linting**|v2.4.0            |https://github.com/pre-commit/pre-commit-hooks
|**JSON Linting**|v2.4.0           |https://github.com/pre-commit/pre-commit-hooks

### Formatting
|Name                |Version                          |URL                         |
|----------------|-------------------------------|-----------------------------|
|**YAML Linting**|v2.4.0            |https://github.com/pre-commit/pre-commit-hooks
|**JSON Linting**|v2.4.0           |https://github.com/pre-commit/pre-commit-hooks
|**Shell Format**|v1.11.0           |https://github.com/jumanjihouse/pre-commit-hooks
|**Shell Check**|v1.11.0           |https://github.com/jumanjihouse/pre-commit-hooks

## Setup

### Developer(s) Machines Setup
Run```pip install pre-commit``` on the developer machine for the pre-commit hooks to work.

### Repository Setup
Create a new repository, remember *DO NOT* include any README otherwise it creates a master branch!

Run:
```
git remote add base <urlToThisRepo>
git fetch base
git merge base/master
git push origin master
```

This pulls the content of the base repo into the new repository - similar to copying files from one directory into another but this has the added bonus that if a change is made to the base repository, we can pull those changes in and have the full commit history to go with it.

To install pre-commit run ```pre-commit install```.

## How to use
Make a change and commit your changes, this will run the pre-commit hooks.

### How to bypass
This is only to be used in an emergency as it will bypass the pre-commit hook checks.
```git commit -m "<message>" --no-verify```
