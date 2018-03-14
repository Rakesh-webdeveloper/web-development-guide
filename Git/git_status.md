## Git Status

_To check the status of the working directory_
```
git status
```
_To check the modified files in a working directory_
```
git status -s
```
_To show all Untracked files_
```
git status -u
```
_To check the modified files in a working directory of perticular branch_
```
git Status -b
```

## Git log

`git log` displays committed snapshots
list the project history, filter it, and search for specific changes.
While git status lets you inspect the working directory and the staging area,
git log only operates on the committed history.

_To display limited log_
```
git log -n  <limit>
```
_To show a commit message in a single line_
```
git log --oneline
```
_To see  which files were altered and the relative number of lines
that were added or deleted from each of them_
```
git log --stat
```
_To see the full diff of each commit_
```
git log -p
```
_To show the commits for the specified files_
```
git log <file>
```
_To show only commits that occur between `<since>` and `<until>`_
_Both arguments can be either a commit ID, a branch name, HEAD, or any other kind of revision reference._
```
git log <since>..<until>
git log 3157e..5ab91
```
### Using Filter
_Search for commits by a particular author. The <pattern> argument can be a plain string or a regular expression._
```
git log --author="<pattern>"
```
_Search for commits with a commit message that matches <pattern>, which can be a plain string or a regular expression._
```
git log --grep="<pattern>"
```
_Some other example_
```
git log --author="John Smith" -p hello.py
```