## create a git repository

 - 3 ways of creating a repository
    - Create an empty repository
    - Cloning an existing repository
    - Adding exists working directory to the git
    - Creating a Bare repository
    - Creating separate git directory

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
_git init templates_
_Initializes a new Git repository and copies files from the  <template_directory> into the repository_
```
git init <directory> --template=<template_directory>
```

#### Cloning a existing repository

- Cloning a local or remote repository
- Cloning a bare repository
- Using shallow options to partially clone repositories

_Cloning an existing git repository_
```
git clone <url>
```

#### Adding exists working directory to the git


#### Creating a Bare repository
_To create a bare repository_
```
git init --bare <directory>
```
- git init

- git clone

### Creating a separate git directory
```
--SEPARATE-GIT-DIR=<GIT DIR>
```

Creates a text file containing the path to <git dir>. This file acts as a link to the .git directory.
This is useful if you would like to store your .git directory on a separate location or drive from your
project's working files. Some common use cases for --separate-git-dir are:
- To keep your system configuration "dotfiles" (.bashrc, .vimrc, etc.) in the home directory while keeping the .git folder elsewhere.
- Your Git history has grown very large in disk size and you need to move it elsewhere to a separate high-capacity driveSSSS
- You want to have a Git project in a publicly accessible directory like `www:root`

You can call git init --separate-git-dir on an existing repository and the .git dir will be moved to the specified <git dir> path.
```
--SHARED[=(FALSE|TRUE|UMASK|GROUP|ALL|WORLD|EVERYBODY|0XXX)]
```