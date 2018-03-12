## Git Log

Reviewing the history of the git repository using `git log` command

Note :
- By default, `git log` will only show commits for the currently selected branch.

_To check the log/history of the committed files_
```
git Log
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
_To get the shortest  form of the log list_
```
git log --oneline
```
_To check the log for the perticular period_
```
git log <since>..<until>
```

_To check the log with stats_
```
git log --stat
```

_To check n_
```
git log --name-stat
```

```
git log --pretty=short
```

_view all commits across all branches_
```
git log --branches=*
```

_View the log for a branch_
```
git log <branch_name>
```
