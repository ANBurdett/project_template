# Project Template

This is a basic project template.

## Set Up

- Open a terminal in Atom.
- Navigate to where you want to create the project and make the directory. e.g.

```
$ cd Documents
$ mkdir [Your_project_name]
```

- Create a README file via the terminal `$ touch README.md`

## Virtual Environment Set Up

Virtual environments and libraries are managed via poetry. Use poetry when see pip online.

- Run `$ poetry init` to create the poetry toml file.
- Run `$ poetry install` to create the virtual environment (.venv).
- Activate the virtual environment `$ . .venv/bin/activate` (Use `$ deactivate` to disable the environment.)

### Adding a Python Library With Poetry

```
$ poetry add [package_name]
```

This will add the package_name to the pyproject.toml file.

## Git Set Up

- Initialize the repository `$ git init`.
- Add a git ignore file `$ touch .gitignore`.
- Add any files or directories you do not want git to track to the gitignore file.
e.g. gitignore file should contain:

```
.venv
*.dta
```

- Create the first commit by adding our files and committing to git.

```
$ git status #checks file status
$ git add . #. implies add all changes
$ git commit -m "your message here"
```

## Publish/Push the Repo to Github

- Create the project on github.com
- Add the origin remote to the local project.

```
$ git remote add origin https://github.com/ANBurdett/project_template.git
$ git branch -M main
$ git push -u origin main
```

- Push the master branch to github.
