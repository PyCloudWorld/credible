## Getting started

1. Clone repository

    ```bash
    git clone git@github.com:PyCloudWorld/credible.git
    ```

2. (Optional) If you use [`conda`](https://www.anaconda.com/) for managing your python environment, create a new python environment

    ```bash
    conda create -n credible python==3.12
    conda activate credible
    conda update --all
    ```

3. Install poetry

    ```bash
    pip install poetry
    ```

4. Install all relevant packages

    ```bash
    poetry install
    ```

5. Install the pre-commit git hook scripts

    ```bash
    poetry run pre-commit install
    poetry run pre-commit install --hook-type commit-msg
    ```

6. (optional) Run pre-commit against all the files

    ```bash
    poetry run pre-commit run --all-files
    ```
6. Run django

    ```bash
    poetry run python manage.py runserver
    ```
## Commit Message Format

We make use of the commitizen message format. Use one of the following prefixes to describe your changes:

```bash
build   : Changes that affect the build system or external dependencies
ci      : Changes to our CI configuration files and scripts(example : azure pipeline)
docs    : Documentation only changes
feat    : A new feature
fix     : A bug Fix
perf    : A code change that improves performance
refactor: A code change that neither fixes a bug nor adds a feature
style   : Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
test    : Adding missing tests or correcting existing tests
chore   : Other changes that don't modify src or test files
revert  : Reverts a previous commit
```

## create a new repository on the command line
```
    echo "# credible" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin git@github.com:PyCloudWorld/credible.git
    git push -u origin main
```
## create a new branch from main by command line
```
git checkout main
git pull origin main
git checkout -b <new-branch-name>
```
## to list all local branches in your Git repository, use the following command:
```
git branch
```