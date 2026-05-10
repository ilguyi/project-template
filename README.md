# Python Project Template

## Introduction

## Installation

### 1. Edit `pyproject.toml` file

* `name`: change the new project name
* `python`: modify python version you want (requires-python = ">=3.12")

#### 1-1. change project directory

```bash
git mv src/project_name src/<new_project_name>
```

#### 2. install uv (if not already installed)

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

#### 3. set python version

```bash
uv python pin 3.12
```

#### 4. create virtual environment and sync dependencies

```bash
# Create virtual environment with custom prompt name
uv venv .venv --prompt <project_name>
# Sync all dependencies (including dev dependencies)
uv sync --all-extras
# Activate the virtual environment
source .venv/bin/activate
```

#### 5. Alternative: install only production dependencies

```bash
# If you only want production dependencies (without dev dependencies)
uv sync --no-dev
```

#### 6. `pre-commit` install

```bash
pre-commit install
```

## Quickstart

## Usage
