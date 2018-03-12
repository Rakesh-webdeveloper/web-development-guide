
## Git Add (The Stating Area)

Git Add
- ```git-add``` - Add file contents to the index.
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

**Options:**
> Add all changes in the working directory to the next commit, including new files and deletions:
```
$ git add -A
```
Add all changes to tracked files and all new files to the next commit, but do not add file deletions:
```
$ git add .
```
Adds all changes to tracked files and all file removals to the next commit, but does not add new files:
```
$ git add -u
```
Walks through changed files and prompts user for add option. Does not include new files:
```
$ git add -p
```
