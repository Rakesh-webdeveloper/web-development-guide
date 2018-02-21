# Git Add (The Staging Area)
***
#### Adding file to Git

Git Add
- ```git-add``` - Add file contents to the index.
- This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit.
- The "index" holds a snapshot of the content of the working tree, and it is this snapshot that is taken as the contents of the next commit
- The ```git add``` command adds a change in the working directory to the staging area
- Changes are not actually recorded until you run git commit.

**Note:**  
- The ```git add``` command will not add ignored files by default.
- ```git add``` needs to be called every time you alter a file, whereas SVN add only needs to be called once for each file
- By default, git status will automatically refresh the index, updating the cached stat information from the working tree and writing out the result.

Example:
```
git add <file name>
```
Usage :  
_Add the file to index_
```
git add hello.py
```
_Add all files to index_
```
git add .
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
