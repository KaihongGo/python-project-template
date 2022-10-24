# Example blog demo

## development

### environment

```bash
poetry config virtualenvs.in-project true
poetry config virtualenvs.prefer-active-python true

pyenv local 3.8.10
poetry init
poetry add --group dev isort flake8 black pre-commit ipykernel
poetry add --group test pytest pytest-cov pytest-mock pytest-asyncio
```

vscode: Developer: Reload window to activate the virtual environment

### pre-commit

```bash
pre-commit install
pre-commit autoupdate
pre-commit run -a
```
