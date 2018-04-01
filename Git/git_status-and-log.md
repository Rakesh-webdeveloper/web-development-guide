## Inspecting a repository
1. To check the status of the tracked and untracked files (Staging Area)
2. To check the history of the committed files (HEAD)

#### To check the status of the tracked and untracked files (Staging Area)  
## Git Status
_To check the status of the working directory_
```
git status
```
_Short Status_
```
git status -s/--short
```
_To show all Untracked files_
```
git status -u
```
_To check the modified files in a working directory of perticular branch_
```
git Status -b
```
_To view all the changes made_
```
git status -v
```
#### To check the history of the committed files (HEAD)
#### Viewing the Commit History
## Git log
- Reviewing the history of the git repository using `git log` command.
- `git log` displays committed snapshots
list the project history, filter it, and search for specific changes.
- While git status lets you inspect the working directory and the staging area.
- `git log` only operates on the committed history.

Note :
- By default, `git log` will only show commits for the currently selected branch.  
_To check the log/history of the committed files_
```
git log
```
#### Limiting Log Output
_To display limited log_
```
git log -n  <limit>
```
```
git log --since=2.weeks
```
_To check the last five committed history_
```
git log -n 5
```
_To see the changes of the files_  
_`-p` parameter triggers that the diffs of each commit is shown_
```
git log -p -n 2
```
_To show a commit message in a single line_
```
git log --oneline
```
_To check the log for the particular period_
```
git log <since>..<until>
```
_To see  which files were altered and the relative number of lines
that were added or deleted from each of them_
- the `--stat` option prints below each commit entry a list of modified files, how many files were changed, and how many lines in those files were added and removed.
- It also puts a summary of the information at the end.

```
git log --stat
```
_View the log for a branch_
```
git log <branch_name>
```
_view all commits across all branches_
```
git log --branches=*
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

_To check n_
```
git log --name-stat
```

```
git log --pretty=short
```

```
git log --pretty=oneline
```
