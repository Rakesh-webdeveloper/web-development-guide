# Git Add (The Staging Area)
# Tracking New Files

## Git Add (The Stating Area)

Git Add
- ```git-add``` - Add file contents to the index.
-  To begin tracking new files, to stage files.
- This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit.
- The "index" holds a snapshot of the content of the working tree, and it is this snapshot that is taken as the contents of the next commit.
- The ```git add``` command adds a change in the working directory to the staging area
- Changes are not actually recorded until you run git commit.

**Note:**  
- The ```git add``` command will not add ignored files by default.
- ```git add``` needs to be called every time you alter a file, whereas SVN add only needs to be called once for each file
- By default, git status will automatically refresh the index, updating the cached stat information from the working tree and writing out the result.

**Syntax:**
```
git add [options] [<File_1>] [<File_2>] . . . [<File_n>]
```

_Add the individual file to index_
```
git add hello.py
```
_Add the whole directory to the index_
```
git add <directory name>
```
_Adds content from all *.txt files under Documentation directory and its subdirectories_
```
git add Documentation/\*.txt
```
_Adding content from all git-*.sh scripts_
```
git add git-*.sh
```
_Add all files to index_
```
git add .
```
_Add all changes in the working directory to the next commit_
_Including the untracked, deleted , modified and .gitignore files_
```
$ git add -A
```
_Add all changes, only for current directory_
```
$ git add .
```
_To don't want to add the untracked files_
```
$ git add -u
```
_Not to add the deleted files to git index_
```
git add --no-all <dir_name>
```
_Walks through changed files and prompts user for add option. Does not include new files_
```
$ git add -p
```
