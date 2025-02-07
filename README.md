# Python3 Enviornment
My basic environment setting to develop Python code.

# List of all
- pyenv
- poetry
- isort
- black
- flake8
- pyright
- pytest
- pydantic-settings

# Creating a Basic Python Environment
- [./docs/setup_environments.md](./docs/setup_environments.md)

# Virtual Environment
## Create
```sh
poetry install
```

## Activate
```sh
source .venv/bin/activate
```

## Deactivate
```sh
deactivate
```

# Lint
```sh
poetry run format-code
```

# Test
```sh
poetry run check-style
poetry run pytest
```

# Build Packages
```sh
scripts/build
```
