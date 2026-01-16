# Guidelines

## Build, Test, and Development Commands
* Assume you will be using a uv environment with a pyproject.toml unless otherwise stated so project files will be run like "uv run python FILE.py"

## Coding Style & Naming Conventions
* Follow PEP 8 with 4-space indentation and keep modules ASCII-only.
* Prefer type hints.
* Add explicit Google-style docstrings (Args/Returns) for functions that include function purpose.
* Add concise comments only when logic is non-obvious.
* Comment code sections for educational purposes especially function purpose.
* Configuration constants should live near the top of files
* Favor descriptive snake_case for variables and lowercase filenames (e.g., power_law_result_dict.json).
* Use DiskCache if cache is used or requested unless explicitly overriden
* If argparse is used, place argparse parsing in main() unless explicitly overriden
* If pyproject.toml present, then use black and flake8 if present for formatting and linting, otherwise use ruff
* Prefer f-strings
