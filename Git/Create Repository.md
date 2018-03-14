## create a git repository

 3 ways of creating a repository
    - Cloning a existing repository
    - Create an empty repository
    - Adding exists working directory to the git.
    - Creating a Bare repository

### Create an empty repository
_To create an empty repository_
> It creates a new .git subdirectory in your current working directory.
This will also create a new master branch.
```
git init <repo_name>
```
_Versioning an existing project_
>first cd to the root project folder
```
cd <dir>
git init
```
_To create a .git directory outside the working directory_
```
git init --separate-git-dir <dir_path> <file_name>
```

#### Cloning a existing repository

- Cloning a local or remote repository
- Cloning a bare repository
- Using shallow options to partially clone repositories

_Cloning an existing git repository_
```
git clone <url>
```

#### Creating a Bare repository
_To create a bare repository_
```
git init --bare <directory>
```
- git init

- git clone