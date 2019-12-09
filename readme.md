# Documentation

## Purpose

To have a template repository with the minimum required pre-commit hooks ready to ensure developers are able to work without obsticles from security and linting checks but also a customisable platform for them to build on to help improve code quality.

### Technology
We're using Pre-Commit Hooks and configuration from [https://pre-commit.com/](https://pre-commit.com/)

## History

|Version                |Author                          |Changes                         |
|----------------|-------------------------------|-----------------------------|
|v0.1|Gareth Evans            |Initial Version|

## Under the bonnet/hood

### Security Tools
|Name                |Version                          |URL                         |
|----------------|-------------------------------|-----------------------------|
|**Detect Secrets**|v0.13.0            |https://github.com/Yelp/detect-secrets|

### Linting/Validation Tools
|Name                |Version                          |URL                         |
|----------------|-------------------------------|-----------------------------|
|**YAML Linting**|vx.x            ||
|**JSON Linting**|vx.x            ||

 ### Formatting
|Name                |Version                          |URL                         |
|----------------|-------------------------------|-----------------------------|
|**YAML Formatting**|vx.x            ||
|**JSON Formatting**|vx.x            ||

## Setup

### Developer(s) Machines Setup
Run```pip install pre-commit``` on the developer machine for the pre-commit hooks to work.
### Repository Setup
*You will only need to run this once against the repository on first setup.
To install run ```pre-commit install``` to install pre-commit files into the repository.

## How to use
Make a change and commit your changes, this will run the pre-commit hooks.

### How to bypass
This is only to be used in an emergency as it will bypass the pre-commit hook checks.
```git commit -m "<message>" --no-verify```
