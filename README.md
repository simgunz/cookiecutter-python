# Cookiecutter template for python

My opinionated cookiecutter for python projects.

WARNING: it is still a work in progress.

## Features

| Task                 | Tool                                                    |
| -------------------- | ------------------------------------------------------- |
| Common style         | EditorConfig                                            |
| Pre-commit hooks     | pre-commit                                              |
| Autoformatter        | black with experimental string processing (`--preview`) |
| Testing framework    | pytest                                                  |
| Test mocking         | pytest-mock                                             |
| Version management   | bump2version                                            |
| Editor configuration | vscode with suggested extensions                        |

## Initialization

1. Create a new project based on this template

    ```bash
    cookiecutter https://github.com/simgunz/cookiecutter-python
    ```

2. Commit all the files

   ```bash
   git init
   git add .
   git commit
   ```

3. Generate the poetry (or pipenv) lock file

   ```bash
   poetry install
   ```

4. Commit the lock file

   ```bash
   git add poetry.lock
   git commit
   ```

5. Install the commit hooks

   ```bash
   poetry run pre-commit install
   ```

6. Open VSCode and install the suggested extensions

## Usage

- VSCode should automatically detect the virtual environment (otherwise use `Select python interpreter...` to select the correct venv)

- To perform actions in the shell, explicitly activate the virtual environment

    ```bash
    poetry shell
    ```
