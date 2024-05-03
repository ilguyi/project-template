# Python Project Template


## Introduction


## Installation

#### 1. Edit `pyproject.toml` file.
* `name`: change the new project name
* `python`: modify python version you want

#### 1-1. change project directory
```bash
git mv project_template <new_name>
```
#### 2. set python version
```bash
pyenv local 3.xx
```
#### 3. set the virtualenv based on current python version using `poetry`
```bash
poetry env use python
```
#### 4. install project using `poetry`
```bash
poetry install
```
#### 5. activate virtualenv
```bash
poetry shell
```
#### 6. `pre-commit` install
```bash
pre-commit install
```


## Quickstart


## Usage
