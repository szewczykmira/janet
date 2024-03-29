# janet
Template python repository


## Requirements:
1. Project is running with python 3.9+
2. [Poetry](https://python-poetry.org/docs/) is required to work with dependencies



## Set up project:

1. Clone your reposiotory:
```sh
git clone git@github.com:{username}/{repository_name}.git
```
2. Enter the repository and create virtualenv with python 3.9
```sh
cd {repository_name}
mkvirtualenv -p python3.9 {repository_name}
# If you use just virtualenv then: virtualenv {repository_name}
```
3. **[Optional]** you can update project's name in `pyproject.toml`
4. Install dependencies
```sh
poetry install
```
5. Install pre-commit hooks
```sh
pre-commit install
```


## Running tests
```sh
pytest
```

- running test with checking test coverage
```sh
pytest --cov={repository_name} tests/
```


## Exporting requirements
You can export requirements with `poetry export > requirements.txt`
