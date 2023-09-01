# pypoetry-template

This is a [Python-Poetry](https://python-poetry.org/) template project for private research use.
Some conveniences are already set up, e.g., [Jupyter Lab](https://jupyter.org/).

## setup

First, change the name "pypoetry-template" to your project name.
Check:
- `pyproject.toml`
- `pypoetry_template/`
- `github/workspaces/ci.yaml`

Now it's ready to setup the project.
Run the following command.

```sh
poetry config virtualenvs.in-project true && poetry install
```

Before starting development, I recommend installing [pre-commit](https://pre-commit.com/), which does large file checking, auto-formatting, etc.

```sh
pre-commit install
```

## utilities

### start jupyter lab

```sh
poetry run juypter lab
```

### pytest

```sh
poetry run pytest -s
```


## Notes

- GitHub Actions automatically perform [pytest](https://docs.pytest.org/).
- I often write experimental scripts in `scripts/`.
