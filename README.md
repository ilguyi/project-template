# Python Project Template

## Introduction

## Installation

### 1. Edit `pyproject.toml` file

* `name`: change the new project name
* `python`: modify python version you want (requires-python = ">=3.13")

#### 1-1. change project directory

```bash
git mv src/project_name src/<new_project_name>
```

#### 2. install uv (if not already installed)

[uv](https://docs.astral.sh/uv) is an extremely fast, Rust-based Python package
and project manager that replaces pip, pip-tools, virtualenv, and more.

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

#### 3. set python version

```bash
uv python pin 3.13
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

#### 6. `prek` install

[prek](https://prek.j178.dev) is a fast, Rust-based reimplementation of the
pre-commit framework. It reads the hook configuration from `prek.toml`.

```bash
# Install prek as a uv tool
uv tool install prek

# Install the git hooks
prek install
```

## Quickstart

## Usage
