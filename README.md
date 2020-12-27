# Project Template

This is a basic project template.

## Set up - Cloning (preferred)

- Clone the repo

```
$ git clone https://github.com/ANBurdett/project_template.git #[optional new local name]
```

- Update .toml file with new project name.
- Run `$ poetry install` to create the virtual environment (.venv).
- Activate the virtual environment `$ . .venv/bin/activate` (Use `$ deactivate` to disable the environment.)

### Git Configuration After Cloning

After cloning the repo we will need to change the origin remote so that we don't push code to the project_template.

- Delete the .git folder.
- Initialize the local repository `$ git init`.
- Add/update any files or directories you do not want git to track to the .gitignore file.
- Create the first commit by adding our files and committing to git.

```
$ git status #checks file status
$ git add . #. implies add all changes
$ git commit -m "your message here"
```

### Publish/Push the Repo to Github

- Create the project on github.com
- Add the origin remote to the local project.

```
$ git remote add origin https://github.com/ANBurdett/new_project.git
$ git branch -M main #renames master branch, main branch.
```

- Push the main branch to github.

```
$ git push -u origin main #pushes the main branch to the new remote.
```

---

## Set Up - From scratch

- Open a terminal in Atom.
- Navigate to where you want to create the project and make the directory. e.g.

```
$ cd Documents
$ mkdir [Your_project_name]
```

- Create a README file via the terminal `$ touch README.md`

### Virtual Environment Set Up

Virtual environments and libraries are managed via poetry. Use poetry when see pip online.

- Run `$ poetry init` to create the poetry toml file.
- Run `$ poetry install` to create the virtual environment (.venv).
- Activate the virtual environment `$ . .venv/bin/activate` (Use `$ deactivate` to disable the environment.)

#### Adding a Python Library With Poetry

```
$ poetry add [package_name]
```

This will add the package_name to the pyproject.toml file.

### Git Set Up

- Initialize the repository `$ git init`.
- Add a git ignore file `$ touch .gitignore`.
- Add any files or directories you do not want git to track to the .gitignore file.
e.g. .gitignore file should contain:

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

### Publish/Push the Repo to Github

- Create the project on github.com
- Add the origin remote to the local project.

```
$ git remote add origin https://github.com/ANBurdett/project_template.git
$ git branch -M main #renames master branch, main branch.
```

- Push the main branch to github.

```
$ git push -u origin main #pushes the main branch to the new remote.
```

---

## Committing During Project Work

The above detail how to set up a project. The following sets out how to commit changes during the project.

- Make changes and save locally.
- Check if there are files to be committed.

```
$ git status
```
Anything in red, is waiting to be added/staged.

- Add/stage the files.

```
$ git add .
```

- Check what is waiting to be committed.

```
$ git status
```

- Commit the files to git.

```
$ git commit -m "Add message (why?)"
```

- Push the changes to github.

```
$ git push origin main
```
